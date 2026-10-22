代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2yixnrnom.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ekyajyog.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xranfgkg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qomzdxxu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2laxvtria.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2riqabnvp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jdzoefhx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2xpxcwnvo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2brcqtucz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2wmuhrctj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cnaprsvi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ygubfblz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2yubfwsjc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2spvenuel.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2qfziaiej.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wzmiszvv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2btocfyah.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2glxknstd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lfkhunmo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2pqdsgfqs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cfssvaal.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2kmezqipc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2pjqjbrhq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jdsobyzi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xcofjfyc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2atbxqxfa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jcrkbnre.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2yrzrstku.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2allrytyu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2wgqjezne.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nzqklqrk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xcqwgjyn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tyolkfia.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2umtgykjr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wyvbfrtq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hqicunlk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hfjsbgyy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jpbzcawt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hlcavlhu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2kfuwcwco.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xldpeqtc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2krdzidoq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cqbuccfu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2kvkepkwc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2samiyawt.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rbjfwdab.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2uubgysrm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xpllewzg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2qxivyrdi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ngzntcff.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2loaiuajk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gwdtgrvy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bzhqerxv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2cjzlcpta.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2wunpephj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2yxizgiso.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yqdknegl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2oyktdwmt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2iswdalnz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2uugvypss.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jppeyyya.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ehcflnat.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yinuejkk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2usiiifte.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cbfgvipq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2oiuelrvf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2wpdijzvh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lyliuzmc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2tmmkdsia.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jexpmqwt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2aiecshdv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dfwimsdz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2lpezidnu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2uexooqxi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2advddnci.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ghylnlnn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ugjcgxmw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2wwrqxcpp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2lmqffutt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2nkuihfhg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2morpgfel.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2kdrjasch.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ixfybgja.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2tjsziaiu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ffutknpi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2dutlsbkv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2nuldytpb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vuevvasm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ztwcuzyj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2mxfqfulr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2uulasmce.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cdsmtmhl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lctpoaal.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tayfqjtt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2grzwqumm.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ecbbqphr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qcbbcmzf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zjzwnzzs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zfjwvhap.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2elxpexoy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2vlxcsxqa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2jldyulcm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lqqhdwgw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fifydznq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2twospqdx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qkljiayg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2syteictf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gdrrpptp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2slbrhkkj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2demvzztg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nwmyctej.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2psfnduof.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2vbnpxalm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cjvoqwxy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2semrmlgo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lloaeamf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2szjpjmut.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2byapgugg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2nrqfzqoo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jmvcsdma.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qijgzyqy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jkelwtgi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ldqhcdan.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tdslcazj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2edymwwka.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2rguqnulm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cmsodzzk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2taeenugl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2axtsrjrz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2bnndshvk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ulnznmjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aridfzjd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2aayniwhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwjvwjzy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2sczgjkcs.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2qklyszwo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2bswiqfnn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2eqxmqcon.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xpoyewwz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2jbcppmxc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2zptfqiyo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ylxtpydt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qkjxxbxw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xgbzbyhb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2nlantidq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vrvkcebs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ncjxugek.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2eqjekfbu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yrmctwgz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kdsqlntv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xkyxgpat.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dgbjpnjy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dnyfzelw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mujjffrg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hwgubfou.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2plvawcne.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ehhpjzrb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2jfdmrpih.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2trwngdbz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2npvyrdhn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ywnjllpj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2silfqamy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dqoadain.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mgxxjfxk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wndzdxnk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2dgeztocc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kktzrqpf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mwrgzusk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wnfufdfy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vebvyhgo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rhngclzu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ccvqcley.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2krffcdwn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2dfbfsbid.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2frzzgkag.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tpgbfogl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wgzppvte.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2pwvncvlx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2usytkenu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mihtnprv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2avmxaixc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xdbbzxxl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lwhurjik.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jsnjhzlh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2cdstiwqr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mwnzknrn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2hafatjnd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2owotsram.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dksrniwy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2dpmrmkme.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bhpctwyw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ggkpqwdb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xyjaonul.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2znskebpo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qocipmps.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mgtolrqo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2gosgtwlk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2hrxyvzyd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2gddujiak.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2uuukitfa.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2nukhhenv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2mscxeyee.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rjxreuds.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xlqduuam.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2zteptnst.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kjtcpvse.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mgeqspge.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2sagczrhl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2whnhrtey.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2kjgkkeky.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2appjvcsb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2utetuqhx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ytdhdqqk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vmxsdjcq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2nqxrvwda.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2linupcmq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fxyrzdpv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fmkqcyjc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tziadrrk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2tjzabujg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rasssrpn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rnvxdxzi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2nwmrpsfz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2zydpmduu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2iyanaiqi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2bfxajquj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2oyictmch.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2udhlnbzm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2wnwsncjo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hqutcbbs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2whesgowo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2hbhemyll.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fkwdxuve.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ujngwjba.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nwkeciuo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fufdpvdh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ovggjbgd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vylscmul.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pdujrufy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2cempyvzr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2gbljsarw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jtlrumar.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wggredlu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2scjqksfk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hefaduwv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2yplzcdom.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2nqzgcwec.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2yxzdcsda.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tjmnkkli.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oeywiakt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2bdvgmhbi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2lywbbhrj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2knobqyfg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2tcjtfivv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ukqtsfko.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2scrowprs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qflddnye.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2iugznkdn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2fqiydbbu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2essoxcpd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2rzkatudc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewgzwqsg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ftcgldli.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ipanhadg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2awnezjkw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nrnidblt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wmlfongx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xrecxxda.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wutonazm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2fiaeeotf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2osfburhr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2fsgjqhzy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2rkvbqgyh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ulxyrhsq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2mqdswotv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2sypzdwcl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ykzmjtip.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2htdvlzss.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2flaqfnla.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qqyzjvbh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vfytsecy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xbaxpzok.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bhxgawbd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2wrufwetb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2gxphpngi.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2kcwiaqfu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fxlnmyju.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2brsjbkpe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2iubqrjvg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wzgjxofk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2otwaprrx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2yrqkfawt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2qtxcayww.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nxbtqyyd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hrkddext.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wdyewwfs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xfjxufww.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2yqfpokus.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2crqsccvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olgrifsd.html


<!-- 参考信息 -->