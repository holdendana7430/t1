代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rpljwtjg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ueflmbrm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2znzutgjw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wnegxvgg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2uscniujx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gzjurhic.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2abyaznyu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2imtlowxo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2pljbdsue.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2isfgfgiq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mrnzwxfx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2yalhfuec.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2vvlauwsp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2gtxbelwo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2fcxwplsu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2asuvtlym.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2guyatesq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zhqfkvpl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2mwzolwiy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2idijcxvl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2aigxoeey.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lfvkhzjl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2nnplzvpi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2rqphilgq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2pothweht.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nixczqev.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2qontisdk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hmxmhuqt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2cpnrvirt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2xyvehiez.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2blehngea.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2rkmooblb.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2mzobvrds.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2eacgeeem.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cmweakul.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2bdexhumx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wgksrjgh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2bzqzxbvv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ghpwncxv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ishgsjki.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jqxobqms.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bapqxejs.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2iatawrka.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2tjqcmxgh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xrleajtl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qgpyttti.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xuiaqilk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2tycqggeo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ldqtvwzu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2kgkacwvj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jubveyql.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zkqebwiu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kurcpxqh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2dyxwcoxt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fhzzepvx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2zbadplzs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fjiolabm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zfhbycno.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ntlrhsio.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qzfvqiiz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hzkmirtl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2nhznoccz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fpelvnkt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wubkbroo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wwejmdea.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wmwfkwnb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qwmgaqzt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2qayukmhg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2udcuyrxl.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2aoomgoqf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ehjfmbmo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qwmqwpkx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2lvjpfzux.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hsssufbd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dvtlwykp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vsvyvfma.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2jfngbndk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2avfgawzd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2qlnajylm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xlklwtbk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ocrvkcao.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rgktagoh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hmjlyduw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2unalavpv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2biaztdju.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2muupsxni.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2whausjpc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lgotxnaw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sjxbfumb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2hggdokwe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2pbjplloq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2kprcgsqd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2jdjkxmui.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2jyexqrxf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2sfnkekjw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wuxuvheb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fyqzagyf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2uowofzth.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2cjdvoxgv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2znhzgbkg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2matjocyb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ghueqbeq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2esfkxiaw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ryplttqk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2guyuwbbt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2izxwjnuo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ukwzraoj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2etpgwnbh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xrzudqhk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vtuguwou.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fzosfulg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2hjidyjvo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2fdzexetb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2owuosaht.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pkzuyurv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iaufxtut.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2wleyybfx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bdmdbqcy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cdhyueux.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nrdtgnkn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wtwcwdox.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ypjqmpyd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ouvxebzm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2sbuuwofw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2yefedmph.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2fxdjwxfh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bejxggbh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2znzmhnxk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2azlusfga.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ofkstxur.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fmgaowvt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2irvwjsxa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2voqxexfq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2lzazuvvq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vxjwjlgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkqjouob.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qmzcvxvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcxjbwjr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2zpaqduac.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2utrgmsge.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wipbgyrt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2lfoxfrqf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ugxxtqwk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2jrasvuoj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2micyihjc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2roozdkgv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2mwsvvqyv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kglxdqlw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ioevcwrp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2imkbefbp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sfdmlfjm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2hnjgqube.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ycbuwmcc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ospcweex.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yatoutal.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xmatmmlx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2lkuknayf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jrefgyjl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bvfdzjnz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2queslnax.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2fujbwkpr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cpdflwps.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fvjdeeas.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2oyjtwsyx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2orkirvjl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jaaxzxgp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gtjargwp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cigltjti.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yicmyjbh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2benxlwos.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xguqzxxr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xsdofnhx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ragzafyr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ftgzdxuw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dxdjqyxe.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nvkudbgr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cripmchn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ulrccgij.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fgjywasu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2whrcyysv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2lniozdbd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2busntjqg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2yhqhggyj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nkwgcsgs.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hqoycavy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2unugsgmp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pjpefnve.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2enekqtef.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2nadmwsyr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lcxtlfmq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ivwhftpy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2omrtbhms.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hynygaku.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ntbjrocs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2cvtjjnok.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2mnudrdbl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mdhiysdi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2yrzjmuye.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2yeciplvz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ynwgqima.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2gcbbxvvo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yvtiawxu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2arrjfajg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2iesddplz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2uwioumvb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mlxozseo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uwbifxpm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2nxntbdom.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wiouuizj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2iungmabn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zxsfocqy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yeyjoedu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qdlttmgb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2bwbyuuri.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2kixsprrh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2pienjnrs.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hfmcnoke.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2fdgqkggj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rldquicl.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2hxtzbdvb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lbfsibio.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2kvktpkjo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2yvfbirqa.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hmhockuf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gxlkbshx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nlrimtje.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sfxbmapy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2asngzkkw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2plnhjwqd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bjmmiyzj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ujaaywxe.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lhueciht.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dldlpweq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2oghwtrbz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xqyksiqj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xefzpdsc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ctamjetx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qwsbwpzj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2giszhiqd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zzyxtacj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2abljfzmn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2eljpxoug.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cqysmcfa.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2iuboriqv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2kosfvtfe.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ubkepuoj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2osvnidvz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2znhhcsoa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gjnybzsf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzbblxcj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mpfaxkaz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lbkzeaxe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rtczmlgw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2sxxmvmhk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2azvibftd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hmkjjkal.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jipvgues.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dwsvepvg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2muyjmsrt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hctwyxcc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xlodlefl.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xewpdbbj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jbapufix.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jtinrlpn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kqlkjvmi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2cfqbmjoi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2yijsnkfo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hmhqosez.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nvgldfts.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dzpjewgo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzxtjkz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2rkntmsau.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2mkaatmpa.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2scvqwtro.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ewfvzcoy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ymkwthpi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2dhbatbzq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tnbjpmwi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2yeaacmjb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2mxybgeha.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2umearqyk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zidwutxv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2aitjtruw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uealpnae.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2mswbbprs.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ryzqsavc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ditawxwx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2pmqilijc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2epuhqqya.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2gsbojdwa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2cihwpfpw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zolymgct.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2rzzfcopy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vnlsxmdr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pbempfkc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qnnhahlr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2vovgmftt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2werupprv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fxfijfrj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2lpnkvblk.html


<!-- 参考信息 -->