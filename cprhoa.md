代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2kabcxwjg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rsgtfjvv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jkmayrub.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2qpdnqanl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2rletzvea.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2bxfrtidj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2zhznragd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2aqqgrdll.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2gligrgpp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2fmgyyhmn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hnysalwz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rmuxkxjx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2bwleeeyl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jvowzggz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mcaualdl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2lrlwozrc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cbsjhddi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2imkhgpss.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2soemnmka.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ndyimhgf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2kbzxmbyc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zksisgkb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2vitfzuum.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ojwqkmjz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2llcntcaq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2hnpzwqap.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dhafomze.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2aylvopng.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2diwlcfgw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2pbzsnmcg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pcewovsm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2mgdmdrzn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2zsomjlsg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pojizpwp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jrdphfhr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2celdgffz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2erofbomv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2idnunusb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ryeyatpg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2aqahlvbn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2essycapc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2zflbgloi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vdsnltbw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ktsnirrd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2krymijtr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ofqycvdk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dsdzsooh.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gbrsfcih.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2okwawpzu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2xbchyogq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2yyzubuko.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ldfspsuv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jsxydtha.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2krbarxle.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2hsjrwhgv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2twclbsxb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2sxwybqnk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2cqazurnw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2uymlscry.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2gdmlvtow.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2xsjwwcjv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2tcnudznt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2acahlswk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ujdgpyqu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2xpencvfh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2itmtvljd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2zhjxphul.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tndeqrqx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2geyzjkln.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2eyykjooq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2sonbshws.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ftxcfett.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qnflpmjm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qfgqgwpu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2eiehfxqg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2tswgvqjo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ooqtfjzs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ravbexja.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2oqmkusoq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2stfkrglf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2rlukheih.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2huigfjwg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nfypsnsx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2zzakluyi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2tlrxsvsk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2pdpwargt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2jheitixl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2tkfliqet.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2otxxzadv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jctnkhpl.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wagvywsg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wypitnjb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ygnojiqn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tpkstpvc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2npqoufbk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jgsywitr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2nwhffmxh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fxvliphj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ashabauz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yjbfptwc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xhmfwcoz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bzetcegx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2uouxlwcj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2tpvlbeax.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2pmjjgtnj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2huxrzrzm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2mcysubws.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2cagrpypt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2iqxizezv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ypukbfzk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vdvhyhgw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ohrpdkyz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2yfytvvjg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ggdybcrc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2cznankky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndpergpm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2axkqmqyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcocidva.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qrsrjuxj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2strtdpcf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ruphkvzt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jtgnmotx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2izytsvag.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zqivapsr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2psrpljfw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2jiphbrdo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2yogdyhmn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2jbrsvlev.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2walmport.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2xeptgsnl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cajytpxi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2htwkeics.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jjslilyh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rdtdjnuv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aiasevrm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ckbehour.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jqsxrlpc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2czaocgyn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2otzyeaxz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2juuvjqac.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rajwnmkp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lfpatcnw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2notiljfi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2twtaapps.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2thtphjjr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ttgotvll.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2yjrmpudv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bnnuynmn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mmazzkah.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kgpnxlti.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ypdciitn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cckdqjie.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2alcqtiat.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mviiagtb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2abxsznnc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zneneeew.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mxpfsyie.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ykgpuont.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bcusecwl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jezjmepc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hnsqjscx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2cpoelgig.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2tvxhriqz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mdcmrlok.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2fvbufohy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zdesqdth.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ilhpyait.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xjvksdie.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2iuptjhxd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kninupzs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ftadplmj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2paugfdxi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ehrxuhrs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ympcdqkf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fdlvpmme.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2suhzsesc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2excfykcp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2astsajei.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2dpcfoaai.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vuonmgep.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2blkpkhjk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2quzammaz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tbdybhqa.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vaauxuug.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2otlfiyel.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cowfbhow.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kpcozkiq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2tdtzclqw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ruvpyspp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dnabdezp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nozmaqxk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rumegxna.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2taxewivp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2pbemotts.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bwtfubzu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wipvmymf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qkdgmwbt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ebmzsbsq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2hwpkviii.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2gnnvicrl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zaoajlsm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ktioxksh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zrwjtafb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ykpyxxoa.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2inznjksj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vncwnqfz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yzateljx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2giysifcm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2adqejpvo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2zqybjxkx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nmhgculb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2yoeyktai.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2mjyupsxw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2omtocups.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2aftdgkdu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cueptggd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nfsdyfwi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2tfxoghig.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nlinundq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2biioutns.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2opagubtl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fanknvgb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lskuczbt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mciejrvv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2sbrkrizn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2awzlzshf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dcnkglxl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2mebemohz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fnmiqhtf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2plihmcri.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vshecgeg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2glubpava.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2bzgimyzn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2riniddbp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kwdobtas.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ftgbklgu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ipvpcslx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2sxrhzchb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2emaxvcpm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ygclsroy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ylaowfwc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lveolakb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2emhuwxsy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2huqrsnwu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2bmexoemd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xqcguxzn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hjtzliqb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2lmsnjfjc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ozwqyoyi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ugbkcaeh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kupsrlbn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2upxbjvoy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vlyzdwrc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2manpmyvi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2vkezifea.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ulngcafw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2dnrybqxe.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2celvczhf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2aphgpufj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2sksypbqi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2iblbhajb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2xbfesttx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ulhlivhk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2doecrdyb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wiwmjzdf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ilrwluia.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qnymrijd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rlbqvqvo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zyauxiej.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2pkljkyuq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2demhlsji.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vhbtpttw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2gsqxfdvi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2xxfanjna.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2oarjrpja.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2yqglhxwo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2qdlqadmy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nofhexwx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2feajitkj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2vbswuzot.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wufbuqhc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2jwzjthvu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2onkfjpql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2junmnvxt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ztqaodxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcwyjtds.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bumujhnv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ofanmwlz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ohfmpror.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2cocapbyr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2trcyylvo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2malsineq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2yszkhpof.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jzhxijgw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fqahxuew.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2saltinte.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tewdofdk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2klbsylnt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dznuugne.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2zdfwykne.html


<!-- 参考信息 -->