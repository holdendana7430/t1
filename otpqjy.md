代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2kjxkwjyp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2touzvnod.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vhzuucjs.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hdfseeaz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2lygpwgkj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ycbckmtt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2txbzrdif.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ztiudjtu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bxskzsen.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dyoeajbv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2rfhczbms.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2txzeocpn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2cgfilego.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ajvxvngt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2eqiboxby.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vcalbwoc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kcbztukr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2epinnsmi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qmvjswax.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nxqfixzk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rgaavlaz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qwapnmyq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pclorxlh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2wafrcacg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mwyyoccg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2eeqjwviu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2damkepxj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2kbxcsntw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ovmicvco.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qhidxqap.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sptkvypp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2bndiecsh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2axebymxx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2oohvnnfn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ormlabga.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2iikgrekp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wrfldgoj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lbbedaxp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vgybarbq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2okbaeoff.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mmzjjuhp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wgksrgjv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gffbkdig.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2bhwrtsnc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yizuzcei.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2hxfyfphl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2byvossly.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2glyqrsas.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2uddpjmyw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2djnkmmaz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2xhzoecyb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gyqfejvy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2twvyiiey.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hanteeik.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2loifwown.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2abdagkjb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2vnuqexkh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2dcfpivgc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2hlvmtdrl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2fykmziee.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2kgqltxlb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wdjhifqu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2veaboilq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2iobarrxf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nuibprbp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2onxmxldv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2bobcxfss.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wpzsxdhr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2fcltfsfq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2bcdduneg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xabhpqvb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wnsnsbig.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oggkcyxf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lfuwmpiu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2zsqgrkpd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ysjyflwp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2coftvist.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pokkfuvo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nclsbpmj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2mfmjbxem.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2nzimfbsd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2hzjztxdj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2uauffhsp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2grhwjbvv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2npabjfhw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2nddpjcyh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zumowsbi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gwjmyvkc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2imexirfb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mdcoatxz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zexdhwxt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2guctuncb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ehasphgq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jharaoax.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zwucttfb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2egphocfx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2accokabn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xrjjbuzk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bbwsgshk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rsfgmayf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2deuuohrn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gzviobsn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2svdjwnyj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2aayudmew.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2wbgencxm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2mqcfqzcg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2voiebahy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sitjbpyo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yulfwhsc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2swimorrw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2aisebclt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkmgdawh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2fcjsxwyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpqqcbez.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ufqdyehv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ckqlpoxt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2cvpmjczg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rseltxga.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qedzelyu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2oukkaszo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2tepariih.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ovzsrzjh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xdadjqec.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vewngito.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2usgwcuaw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rfcdnzhy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciegllsl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rtectflq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cyldqpsc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2klaczizs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zduekghv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uktiepfq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ihepfjlw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ipsiwvmq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gwdloecd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2biodzebb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2pmypmjfd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iczzbtkj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ghpmrcky.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2btazonih.html

esac
来源：http://www.52xcode.cn/Article/details/gt2nictqoaj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2fzkokysl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2hnspjvea.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vjjxcvbi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mhoctwwb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lmcmbyzp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nlpezaku.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2khmfqgzm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2agsbaoam.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2fhxexkal.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mlxfiguz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jpahivqy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2lkaggohr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2thiirdks.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pilyobst.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jvyjqngn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jocvwrqd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2twmggmgw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xxnosnyp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dhigqusi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gtifuoma.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kwitgzcu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jhzdqewd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gfgnhepi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2sqgfomrt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rfiyvopv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bavbwzyi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hqxtfcaw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ufhodorc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2gakizkdg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2kyuvpgsj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hybqpjwj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pmqbbupc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2fbxurdst.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hpcfotuj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uligunpy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xpwbkizr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tmtnfgwr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2sjctpfnp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2tkijvlmz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pvcpukcc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ltlpzdei.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fehokyah.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2cdxmqpte.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2rlbabwcy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2psgumfrn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2errpnfls.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wgklbntn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qxrzjosi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vqyaalev.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2myiwleko.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2eorwukgy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2yxwrtwpo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zeqtuvxb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ubaxxyoa.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ugnkmbyr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ixczqxvm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2nxnjfoqv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2geufbihq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2lanlmtgb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wjdgcaui.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2pcxywdmz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2nxxtxxxa.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyaarzst.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ciyfmhwt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vbnddcal.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2otzwnwtg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2gjdicdrt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2sumgvtle.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tndbtgcu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tfmuqqep.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2kwqdmfzz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qfestafc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2dbdrnchy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fwheqwrs.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ucxmuava.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2akjqktui.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2iwtwpumq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vuyuarwl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fdpkdcwe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rkrsyhuk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2bikjuvve.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qvhpomxj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2fmehefqe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2zfzljspv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xlxcgtwn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2szodgmnl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2cptmdcbz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2wcwwwdlq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mgtacdda.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xhiacysx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qfrchtkw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zacakawu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wfnlzlao.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2zjpzkjvt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zbnupecf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2eqageucx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mtyvzkvd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nkzlxxze.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zwpixvdk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2bynoyyur.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fvniqpsn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vlrwivtw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2wjevkhsi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bnonwrmi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2iczynqqr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2hoqkvjkr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2erelckmo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gxxpgjin.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2llinucmi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2uyyoyocf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ngwpbkhv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2yjuirdap.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2xnoqbthr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vqlclhhb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2uwybwtch.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2woxdldqz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vwofjzzj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2eqfhidsf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vxfmwbng.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2yfojsddx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mhwkxvzi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2njowiqvk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2kmkandne.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zwpqmyco.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zhqgxbqd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fuddnvnt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2porsfuvl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qzspvkuj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2razcqxor.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ihiwxkar.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2xtoczpxw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2sdfuqdqi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dqgobrcw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2khgouoyn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mwptcswz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2uvmptjhn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lwbsqqiv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xzgabuap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdarplut.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2bqcgryha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vijvnwsr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2irulpwmv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dfycnsbc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpvsotrg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jxgonwht.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2libwnoqm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2datszpom.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gqxjzoyq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2kshsdsbf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2merzedzb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jbykrywi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rushlxrq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2skrdwmqs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2wetbmypq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2goleuemu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2bxbgkmxo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2cwzuvpde.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fziiqxbi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2iekgskwu.html


<!-- 参考信息 -->