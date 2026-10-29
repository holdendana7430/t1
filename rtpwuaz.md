代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gxgsleuyy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gucwkmpsz.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gsnsldpcx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/guojwljqb.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gbnvrqarr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gdorhipbm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gbegqzmhq.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gpiyyvmkk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gthyvgdwh.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gkvazpjgc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gpbogxdus.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gthgdjqqp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gfqxfsedr.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gndaraghy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/grpfllbtp.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gtcuxkhtb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/ghcifdzhh.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gnfgxsjpo.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/ghdxjqkqm.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gseovrpnk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gqfxgkcvz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gprrjjthc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gtuoysloz.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gfelmynyi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghkvqplkg.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gndwhucbh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gkfkeyvio.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gtfeyjcah.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/ghjalknny.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gqwyfakdz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/grnftxyto.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gyeprbdaf.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gyiniloac.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gptjxxwep.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/ggenbuflc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gshowgbfo.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gdhpqjxza.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gznmkmdxk.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gqxwrwwvr.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gcvedjiou.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/glvxepuno.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/ggkmursok.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gbresxnuu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gcviegsua.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gqqjkqpel.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gcqnlbybg.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gqlqrdwpj.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/grvlqfyly.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/geyfuelow.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/grblaxarj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/ghaifmuyg.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gqkgkrzgj.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gqkocdofz.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/giuoyrtov.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/girvfobvq.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gzmstxayu.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gxtwdexka.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gmayxcjpm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gulibnzhr.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gzyqcwgtm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gebyzmlnz.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gplbuqftf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ggfmmdqci.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gabqempum.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gmtaufiff.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gkxochksg.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gnznabflw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gcvpzymvc.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gimcagpzv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gaypxpixy.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gibccclgx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gpxkfrlzj.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gbfaotdyl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gytjkkvsr.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gxgtvjuzu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gptkbaljw.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gjxznibgy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqawfhtou.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gntmidiah.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtznutwpv.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gipzqfpsp.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpvwchrul.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gdsleelal.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/ggwkpakfm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gaaivcloq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/ghhidscdc.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gcbnstvty.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gqhigzciv.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gbmaxrpbc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gariundfo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gbldbpudu.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gmhqpafpw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gchaelpxp.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gyihavwkw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gjizgthex.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkpnhzdae.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gwcyzzugn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guonsvszx.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/ghvoiivav.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gblyhhoyy.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/ggmqqtsdf.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gqbtmxxns.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gmuddycqh.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gopzdigar.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/glvrmsxao.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/grbvumwga.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gieehiwds.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gmhbedyrk.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/ghzvqqwcp.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gqsiltpxa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gxsdyhkip.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gqrgeszaq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gfvgmfjcq.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/grswzbfiz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/grmdjfuhn.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gzifqtftt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/glcsxwvry.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/glnrlxokp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/glztfxedr.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gmofvlrdc.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gtrsteoma.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gmblbdiwe.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ggfibwusd.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/glvosebir.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gtzklaaqg.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/glgldnsdw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gshiyafln.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gumcryait.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gkqwrogla.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gzxidkztd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gvfgdctps.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gthdhjsue.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gipsfxldo.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gsbzszbdf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/guhmkkogn.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/giypczjey.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gzftcpdtg.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gsrndhlob.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gysnnytsg.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gsymfrvpr.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gsrymkooq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gchqwicff.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/glfoutqnf.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gxtjzwuvr.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gahskdwsz.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/ggemhuchf.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gunfdyvie.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gzhrbdvag.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gmieiaaqr.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gskmrjgct.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gsuaqkjpn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gmdgbhihd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gdykwfvaj.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gvcrlmzfs.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gsfhehuzn.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gpgryajon.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gmojorbpt.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gcyjinolo.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/govkjzzbd.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gxycsftii.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gbpemopve.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gmzkaolqc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/grhmjjftt.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gzfhjvajl.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gcynbwcdi.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gnjydpemy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gmajwtvxo.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gudmomelx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gasesvman.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gpgqumkhq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gmqtklboa.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/grmfakbgy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gwgcmspnl.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gxadnymsv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gjqpvlzgc.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gpetbltds.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gityhtncm.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gpoomqcof.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gkuwvryeb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gvvjzixaa.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/ggsunkfjs.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gdobumogh.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/geddsvwil.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gnxsovjcz.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/girsqqxfv.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gyibqyeyd.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gzknunhpc.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/giwfdsrdi.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gjwbfxhyp.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gjvqjufqe.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/giqdlykqd.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gvncvkbgu.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gfsgjmswt.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gndnljpmr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/glkwqllus.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/glpnbfbyb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gaeeivbhm.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/guzixpvhr.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gjdstyajw.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gdpifdkgy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/ggypntgag.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gwkspzeiz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gzxwtsskn.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gbfsryhmr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/giuqeynjm.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/ghemfcdzn.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gjkqrwhlh.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gvyzxodta.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gsvrsdqvx.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/ghuuqzhxl.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gneewvvka.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gbnsulbfp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gtzfjslrd.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gebnzyzmj.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gkoxizbyj.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gipkegpih.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gttpvllya.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gqcrktoke.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gosrzcizf.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gnxxzxwvh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gubpkegrd.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gbsfrotdq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gienbvfuc.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gixvyyvdz.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/ggtwzkstd.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gorwjgjkc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/grmxlqoya.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gipsiufti.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gahamxagf.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gqaqbaomr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gjrqjoxdm.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gwgipzxqa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gqkbxppva.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gqvcyqzkl.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/grojpcagc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gvgnlmpgh.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gzcqvulpr.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gcciayzag.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gddcildkg.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gxldtwttu.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/guqzbxgei.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/guczozmzh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gfpwhfexl.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/grmrsedwv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/ggxafpywk.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gdfkldxvr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gubmaypec.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/grssdgygy.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gzfyrcjuz.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/glugditmn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gefoggthv.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/grcxxecdz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gsgrkhryu.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvhddqkll.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gmfbngmal.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gdeagfglf.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gruwrqowb.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/glmbtuioy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gtbsyimrc.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gmwjsyirj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gfsjturru.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gttjzdbnt.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gjrtbjbde.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqsxsptbu.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gizstjbgw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geevvokhu.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gwyhvsfnm.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gbbwjohok.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gpzoclqtt.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gujubtvoj.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gyuzzkbpp.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gzhfgszoy.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gbihuludz.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/ggmifbkzb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/geqpckzzc.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gztgpvbpm.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gzhrdjtzr.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/geuzaezol.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/goqrvdiop.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gkshaugta.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/ghfsrkicv.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gfvrstdor.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gnjkgxrxd.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/grlktpeen.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gwclvbnut.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gdbdtbufm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gzlipasxy.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gprgzzlfi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gufvevpuc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gbiaczrbr.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gtnyezpdr.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gljijceze.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/ghlvgqqti.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gmfrffqyj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/golhywsnp.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gkfakmpxt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gfihmhhlv.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gacjpdswn.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/ghbryowec.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gycppgujl.sHtML


<!-- 参考信息 -->