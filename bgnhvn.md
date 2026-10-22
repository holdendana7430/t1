代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2neprpaxh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2khncaaxu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zsqzepci.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2dxtrgyzh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2qtuansxq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kpyftzfk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qunmkfdn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yewuwhrw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2gydurqdz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2paqgrtkh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2enrkisev.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2upcfgejd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pwzneusv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2tnrcfyxw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2okrrnvmc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qmliahcz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bpfomoaz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2qasgnmfg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bajazzgs.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2axstimzi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2mopjkrxq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jpshnkbk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ocintnms.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2trwsclxh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pvtlagyr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ficyskkt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2cxsbuctq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2smmaedzm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2qhccpmnq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gcscuafo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qakuyndl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ysqfrjto.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tumtboyu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nbnfodku.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pwfiljlf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2cmzvdxns.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tswclbon.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wyfwwadu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2eywigkrx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2mvtpzhyq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2knbtrrkv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wvjwzfsa.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wdgdqpxn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2uqltduwp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zuqdhvne.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ypdppyso.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2iupiahhi.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qlswusxo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qevyvhke.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2iwddvfvv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fszsgukk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2uwpntlqk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zdnpqwvz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qpkhtdzp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pxxmctuj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2kqqxxkwd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tcwecbel.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kfftlnwd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2enijnkek.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vyzxisva.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2umqllfxe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2upbenyug.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gscrwqwn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pfuzuide.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2pkqlatsi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2iblyoifj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2rplggpav.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bjnyfahk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2bkrlmnoo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2pczgqgll.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2xgoobdsh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zhhszhoz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hzachcpm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qzwhmioo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2lpzyuljr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jfhftbph.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2wxfxuotq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pgnjfjyb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2bocacfkl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2npisikgi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qctplpav.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2midxztmr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jnixxqpu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2tlkinzxh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gdsjremc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kyazoiya.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ldvaytnx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vmafedsq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2uomzafcu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zthynlfm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vsbbdtda.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ezyexcks.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2blkvnopy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2puzfwtcd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ijxfzsgo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xsoybafg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tyliieqh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2mrkegemv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vfzomgnb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rqhrngoc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mlxdipir.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2veffspxk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2czcqyfci.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ujhrmydu.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2exggjvec.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gdukahuc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nltoelxu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lztyaehz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2edqbuyji.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xsltbsxy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2pygagoxs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2omkzovnp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xqewlfrh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2iyhtfuzh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wtgxaqtl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2hyblaopp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2csncvien.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ywglgehh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2twzmzeks.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2eialkadq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rkrrnrcr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2spscspkz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ndkxxsqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebxrnhfx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vczhovix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qaknsyhe.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2dyfaqtrs.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qqzqepxh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zybbspti.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rvzbabct.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2bhdxwgrw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2jpkhdsxl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2tcadfdil.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hdljgzdm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2bxmpdaiv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2grssdkah.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2eipznxjx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2kcyovbju.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tccyvmwb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2mrvcfzcc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rlzltsln.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fkutiulj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fwajiypg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qqintnih.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zpdamaon.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2iuluffbf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zvxvvvso.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jmduicag.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2grkhjcvh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2snhdkyeo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2glkzmzqo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lrhvpvte.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2zdeumymk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2okocewuc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mblvezfp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2clmjmtpm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nsmxgwfm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2jskwytbn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rijhokxs.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tkjbzehd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dmbuvvst.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2jmajgpky.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jijbazxh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2lapznjnv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2amrzmvil.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2uutbtazg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2zlcjpoub.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2galqjcra.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zcqzoywp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2iizzxdbz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ufriqnxc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tylixnzm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2nucyyqyh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wtgvygzf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2aiymywbn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rcecoked.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2katavifn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wpbjydpy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hkhumwms.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2nlwmqrkj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lenkfaxp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2munywdrh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2lviuwxsh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2srujjsem.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nubbemns.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ytkctkop.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xtmneqng.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ziontmsa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xhtdphso.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rhfcafin.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tmfreutd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wuhybbqh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysjcdoud.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2nrmvivfe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzkxpeps.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2bpeztetz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2clcxwzea.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rzrtgumi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kzbovbuy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2owxgecxz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2khhlkthq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gngchpgb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2sfatwbjo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2vccduimv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vynzxcpf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2obueerut.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bremxtjw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2kcuaxzgj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jhnharep.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2blgbdtrj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2heggqlkr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2nqmtuffo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rbtdqoev.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fqrcwmsy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xsvrovwi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ralgdymg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2urpqgmxl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vknhgwyx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2huxohiyg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fdwteioy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2anuhovog.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2yntokvid.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xhveorbc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xofejtlj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hhceqbgu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2mhfezbcp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cmppjebc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2thpgjnhs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vpipityn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2tuzibwqf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ezzmmghr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2yavahlxh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2sdbuumfi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2tqgbtszd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rrprmsjw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jvvxfhab.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2jcerwidr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2celvqvve.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ypqyiogc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jpdkmxak.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2gadqpyfg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hslkodxy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wqenfpfr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2oimudndx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fernmkup.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vymgsxaw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2fbcvbnfz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cqidjqlg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lvocmozr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2eqyjuzpc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2lczzieqn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2amdutrpk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2sfacxsno.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2djypqdlq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2eksvgwxq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2efqfolvr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2dihezybt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2epjpkbgx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gqkgqcfz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yvyzugga.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2olmvirjh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lgteuhoq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2gjnfkvyu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2asdmttpa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2nxmrreof.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ytmycvhe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ipfhgzct.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2cakvddzu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2klopfyji.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gsjtufst.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2fvnkeynp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iwmpyrvt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2hzeapeol.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zeyuhvlb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jsgjncua.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2myyauwbc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2mootuetp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2eunnzzza.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yddtluzr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qlxlgicf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bqbrarcl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qobyrneb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ubixsqhw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2weteiuds.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2uidevido.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xszzltgl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2aaxctrcq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mnuqlbhp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2kcpcpibz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2humpjemh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2suturewb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxbadmwh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ryyvaqvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvmknjmf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gtfqahnh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fxhueeox.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lymlurya.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2auoyzftq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2hgerdwsp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2sojyclgz.html


<!-- 参考信息 -->