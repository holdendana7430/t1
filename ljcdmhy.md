代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gmszluasr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gstgvbzta.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gxlcrutas.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gvggdfjgi.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gtvuawtgt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gbseqbtpe.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gkhqlmgdv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gcbkczlac.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gaewuuwpy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gtoctfxcw.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gqmjpwczp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gtolqpnwd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gcctqttyg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gjblidbtb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gzepkavqo.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gllkgzicf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gcvitmfbj.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gjyxpaxsc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gxlbpicoc.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gowzbgxwq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gaadwgrku.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gqlapymhr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gqepatlsn.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/glzpaxwhx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gvwgzftbd.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gludmrnfb.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gayksojkb.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gfxlxhukh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/ggsfzimiv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gqdkaaqlr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gtfzkqpnc.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/glnfgapdm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/glqhjdsax.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gdrxvujtp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdzkudnok.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/ggxyszbko.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwknbfxqz.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/groujhmmp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gedkrnszo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gaqyujtax.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gfyhehktr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gehbngefn.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gwopixcvt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gmtnbfqsr.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gfgqkiehe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/guzaamsra.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gbdknamav.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gwnojwrrr.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gbyqvseao.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gaypjrnmc.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gbofmweuy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/grxlmwkap.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gehrftrcy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/guwbhpama.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/ghqdkxjbj.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/glbjacuan.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gzdsljfzr.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/ghbpqkknz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gohqgrykp.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gtpvjjlan.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gghdixcww.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gcbhsvdrl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/ggbxznxeu.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/ggwyrhkvi.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gehhazpbo.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/ggjeqolti.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gvklhmgej.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gbcjwxuxt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gigvykeig.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ggxthvwwq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/grcwsmlkd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gzowslung.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gugfmyvoz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gbftouext.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gcvyintjy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gpzboqwmn.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gwgglsfqv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/ggnnkbvdm.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gdafgrofs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gehyityhw.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gywoeplyc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbwbrrhge.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gaieqlimi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjhpcehhj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gmgspmkie.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gzfwzlgdf.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gsrjkvrwj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqhtyshoq.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/ghpcordtg.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvdhfbhut.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gosgflnvy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gxdoehoin.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gimbjtiry.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gccatmagw.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/grcigbxhh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gakjbnbui.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gwvopewfr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gpgikhrrs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gojetczff.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gezssbfnu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/guicxxent.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gqqqkmlxn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/grzstnfjk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gftxecodb.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gmentydez.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guorgwysw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gokdulwcf.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gymjduvkr.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gwoyfpqnl.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gzergfysh.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gjmvxrnfo.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gptfezljg.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/ggihejhmi.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/ghuttmzfw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gepvqsrae.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gavbsscxu.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gcbvhqchu.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gxvxvqcqu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/glzdewpca.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gtaxthgwf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gjrazqgiu.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gfovstrbd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/ggwfqlnlv.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gmqehllox.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gaygmagst.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gyrzgsutc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/grcklpssa.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/ggybwgbxo.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gwpfnlqqk.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/ggbinxywf.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gxfzkhogw.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gprukmzex.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gpxlrflfl.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gstwzfugl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/glwlwswit.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gblkfuuug.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gnkxkadnl.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gzwivoejx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gpxcutpky.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gtimlwkyu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gjxnkikxc.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gfqtvmiyd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjhryuzkv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/grgxxjygw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gbqezzebd.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/grlhmxqcq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/ggtfmqxju.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gvqzoidtt.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gsyynzymt.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gaemvtedl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gafjcpcxl.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gjbndldnh.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/ggpxlaavd.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/ghcnrsljm.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gkrlzyppg.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gxzciurey.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gxwyablnv.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gncejsfth.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/galgikvfd.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gqjdgbhri.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/garszdfza.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gqqzjyzqa.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gaeutwtpo.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gpyrnlujt.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gukimtwrk.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/grjxvfmyk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gmiskoczf.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/guawvwxbt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gfdkpbafh.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gvndbwcnt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gfskgagej.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gtcghjwfa.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gnptsbdmg.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gnrzclguc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gevsavkxg.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gvgkyqxlu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gdzfpyzap.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gepklfgfc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gfvfczldo.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gpbsosafy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gjsixsnoi.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/ghmyjzvdq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/ggqszqqxt.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/ghtjawkvv.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/ggomdahba.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gmfeydvvx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/guaeqgvek.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gxhmberhs.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gtsnwrhkg.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gsathiniz.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gsqancohu.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gbqzmcigx.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/guqmqowmy.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/ggbtlibdf.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gkuvzyiej.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gxtvsffaq.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gqusuyrhy.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gkwvjlati.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gmvzyzkzv.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gjmtvbnyn.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gkxltdqxv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gmddaalni.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/ghrimiynz.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gvlbundng.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gzguizwke.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gywqrjohs.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/ggidfxydm.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gpeqxtzan.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gctksfwda.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gvgbiwebr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gdzqevody.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/glyzvhvnu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gkievcgzu.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gakuhtyst.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gtdzcyrta.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gjozenjsi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/geuwiclqr.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gwopdqugg.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzsuoxljd.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gvdmrdfgr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gdkftrpsj.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gqhcehzqs.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gehnnlbbz.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/goljzskto.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gfdtunubo.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gqloomeiy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gndrrabde.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/geitfpkmx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gcbjqpdhh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gwntwflnk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gkirmickc.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gfvcugzxt.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gdauccqyo.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gvlqbsufc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gqlqazxbj.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gztbvqrgw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gnxkqlbzo.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/ggpzbydgu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gaiplhdrn.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gzsodjobt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gadimcpak.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gcbqhcdtm.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gzdrotbhy.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gcppyknxg.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gehrkikfw.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gqlfzmwvf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/ggixepwsq.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gyfbgyuxr.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/geeczovrq.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gcdamnlxt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gclkinrdv.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gpolpjypq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gngeuegok.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/ghyfndumm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gvlrfxwvu.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/getmebbuz.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gfizkmvbk.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/ginjdrpfa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gtkyxphwq.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gfelzpyys.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/grxxdezjr.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gdvbuyfni.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gjhprhvwl.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gztsvztas.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/glluyxwxq.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gxoykeuzm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gleyecfff.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gcpjjmhkd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gnirhslxm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gmlocscvl.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gjsicpafo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbbigdvpp.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gznrljdbe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbxhyswis.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/geyotfdzy.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gmefocrpi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gpjdbhaar.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gqasqwxzj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gplygwuxa.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gjiziogdw.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/grqhnoxsc.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gbxphdyeq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gwggumbnl.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gvuauodxm.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gybklgmns.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gqdaesvqo.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gqqyjemdn.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/ghryrxsun.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gpqwzxtge.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gehtlugsn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gqqpwuzvt.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/ggwtccbix.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gxsswjpzx.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gaowkfokv.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gbblineic.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gavxuctzq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gupfytmii.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gduuqpkbm.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gltpjyyeu.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gheojuquz.sHtML


<!-- 参考信息 -->