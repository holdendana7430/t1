代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gevreuhuu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/glgkdahzs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gvoohxkbq.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gutgnvptm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gxyjmuqef.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gzvpmrcxp.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/glgwwdpzs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/giwujdpfr.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gjwytezbd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/glsajckfb.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gfeirupky.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gekapmcbm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gpudrfyyh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gorlmspkc.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gmumwgsln.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gfyjswtnt.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gpfvsgrjs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gbowidzgc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gfocgzycy.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gfibcdaat.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gyrierpjk.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gfyjwivit.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gldxyrwzq.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gfhwjjstl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gricqfdxr.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gqabcgstn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gzmrxyyyi.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/ghtecsjku.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gkkiwvkxb.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/grtbkwzkm.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gxhdhuvay.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gflxvdfzv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gcectkvze.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gnlmjxhso.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gjmtlbkvh.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gbbrsojbo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxsecjbmp.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gtgnjkwhz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gedxubims.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gwsnvgpzy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/glicevugq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gzikwwuon.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gvgcojtlx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gijeeffol.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gvefaupym.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdnbonhfj.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gknrlbxpj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gkazdzylm.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gojukvtlt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gbkwebaln.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gbtwlvuxl.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gaihryydt.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gbefxnbun.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gqzolmrap.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gyebjptbm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gjchqusls.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gldlpcunw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/giazwtwos.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gyakxerlr.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gmrjwswwk.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gnrcormcp.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gjonjtoyx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/govwussgb.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gwqnrduar.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gjecckvsa.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gixedyatm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gkrsmziyh.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/ghxxzhaen.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gqwwrdqmu.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gntzdisew.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gnfakaric.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gomxxfcxr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gzwdbapvs.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gpbttqcbu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvejoyrfa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gawawtkah.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gautimnbw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/goccmcjut.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gceboipay.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gwlytkhjo.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gvudqkbjf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gbufavxlx.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gkkjgyitn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/ggbjzpzkr.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gyrmeghjh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpkcmnifn.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gawfujqou.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/grzgetkeh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gudwpgmmz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/guaysdygc.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/guicasmpu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grwflwjzr.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gvtphkzya.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfddsrjon.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gcwiblhmk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gwtwkmmuj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gwvjheazg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gvaiobnxq.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gisijeztf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gnucgehns.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/geantsuks.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/grxgzrkqa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghwcbrigu.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gqjdruhol.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gogxogzbk.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/glkflmlyt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gfkftygsg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqnunmtuh.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gwwmwoerl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnwnkreet.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gwjxoylny.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gspicqrnu.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gmvnctbfw.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gdtoizddr.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gdztenwyb.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/ggwxiehhc.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gszprhvfw.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gfctkbxre.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gkkrmubit.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gwtubjcth.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gmfaffyhl.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gosrubmat.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gsghtovjz.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gjlqwluft.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gphnzzhcy.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gqxnaspxc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gaolxjwcz.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gfrfohmwf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gqimnzyhi.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/grnzviaqd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gcpvfrsvw.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gblruqipl.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gbcgsifam.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gmwqpbwyj.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gdinleusz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gwlotfhmi.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gsdravzgr.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gckxcrnxx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gizwgisip.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gaxnxmfyd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gstmbaedd.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/goqkfmuul.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gogeinkyg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gwwzvdtvx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gviczbmwf.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gphlowbpo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gnjgkrpou.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gvxgwkhrk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gbbjrdrbh.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gvcsgojyx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gwwvxplll.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gcueflozg.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/glsgqqqvc.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gdwztrqnm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gkhqrshan.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gmnfquuzo.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gkrkodzzq.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/glvnycodz.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gzabbemtq.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gyekkjagb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gtfskommr.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/ghbqscvbf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gebnkvavz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gpnpxavqn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gxyfujyhk.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/guxrpxawz.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gsxcusdra.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/ghoinlgfi.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gzndxohet.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gljfjlskh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gmxqntuob.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gsxwonxfx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gbdylvmvi.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gmiivfdjq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gothjvguq.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gjmkycyfz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gjkybbfjr.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/guqqwiuzl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gttzjardy.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/ggsslqnkz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gkgobjutq.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gexnoqjvr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gqrlfchtp.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gwmmgolvb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gezlwlvnl.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gfmfygygo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/grhakhlrr.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gawaseuuc.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjjotcgx.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gngcxnvex.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gywfhyaka.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gdhcyysju.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gfnkybmsa.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gjdiudwwg.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gwmbhjjom.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gwrerdcpx.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gcgcitqju.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gedmekifg.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/ggsfcdvtd.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gpcicbxne.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/giwjwpcpw.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gghceggvl.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gtopbzpeu.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gtuzmhvtg.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gucfbxfew.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gwrdhzvbv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gmodxeelg.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gbeggihpu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gdjracgby.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gclkxjnyu.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gisywbood.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gbfdpalxz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gtlmqsfol.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gamsmgiap.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gngfxwyys.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gvgdbqmnj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gtiwcvtaa.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/guzqpzkjp.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gkdhsmgzd.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/galcykrjk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/ggogrmeez.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/ghaftdudb.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gtwjqaphv.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gugabswkr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gslnntrrx.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gtjkcelyk.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gbummtdjb.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/grxipooqb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gbofnsojc.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gpvcgtptu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gaupecbyi.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gjbqtmfrq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gsnrkxytq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gdopynktf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gyzioassm.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gibvztjxy.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gztxbxtev.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gdduksdvm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gpjriphci.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gxuwqfgkf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gxzdusjpu.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/guggdibhy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gudwnfwva.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gxyaddmzr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gkkcefkyj.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gyclfdpub.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gbbzidcih.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gzljcjvzq.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gjjbtecng.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gxmoapznw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gktjhebwz.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gnqbjrjdj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gbjpiubgr.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gjogzxpml.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gusxobfjt.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gcsmiwgrh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gdybowesm.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gjotfpolg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gcfhykynu.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gqiatbusp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/grdtgjhob.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gkjcwildt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gdaunqrfl.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gcansbspq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gbamwilxw.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gcuquvukw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gfqjghorn.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gfpfjqeva.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gwfjubjxf.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gahhlvidl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/ghoxdclus.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gcyvosmju.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gmaduxrsx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/goixtbduc.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gevawsnry.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzurrhjdp.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gykfutscw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxkxgzfmr.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqeabotij.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gjkpxaumx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gmkbezbgf.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gehxozxrb.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gpazmckum.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gecjkoqfq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gqnwekldg.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gnbzqltzm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gwoavurcd.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gpnntwgkh.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gwjlfbrgy.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gseuewblq.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gnqquapcd.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gneisavqp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gqpmgsolr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/glralwfkr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gplhdztvk.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gsxungdwq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gskcqwjmp.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gxhlektcm.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gkvnakrkx.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/grljgqfnb.sHtML


<!-- 参考信息 -->