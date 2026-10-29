代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/glwlmolnu.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gxdwziruj.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/glrygwrjy.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gzzvibzln.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gfajkuisj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gfjxcjdyz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gdyjqsgsn.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/ggkihyaqp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtqylpepj.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gmteqajtp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gzajyqhsv.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gxdqdbats.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gbmbvuejm.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gmdhtpycu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/giwxzwxvy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gttbkqmql.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gcbuhquvy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gfczhttli.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gsvkyojtr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gyuvrlorl.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/goaxbtqyr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gfseadfqo.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/ggdwfaerc.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gtmxephsp.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gjuytiphg.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gdoawelfw.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gnolopcry.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gxpjomgkn.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gkzwdvqez.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gwotkspqu.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gsfsypxbw.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gqjcvbbdw.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gnevjrfrr.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gjxkunndm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gvvopjbuj.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gxpzvjbfl.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gnztlcsxo.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gtdygfkif.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/glrpvlgiu.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/ghpypnucb.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/guuxdfcea.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/ghhhaocuz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gdneciljb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gagvmigmm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/glnhakmfy.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gczdquwwm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/glubbvpvk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gxnxxawod.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/grywszmtm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gmdsxvotm.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gcxvqkmdf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gkfchbnkg.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gwcjtkxvo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gvavhcjpq.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gxrwfdstn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gakepckbr.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gghostbbo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gtspbhgiy.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/geqaynllb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/geevykfay.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gmfhckykk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpivkrlez.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gbeigqqal.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdwluqwus.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gvlzstedg.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjayechks.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gtyovlbtb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/grjsjpsvy.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gstlfaeyy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gctlseoll.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gcffjfiym.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/ghktqhvhb.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gywkfyxzq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/giljeqxga.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfcbuznkc.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gootceuwe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gfhufiadd.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gofttaiym.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/ghkbnescs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grxhfradh.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gypzlqtag.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbdhixuet.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gnyicxefc.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gpdspitad.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gatzxluai.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gmcrdkcos.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/grsujsdpd.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gixlgskch.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gfswkhtvm.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gsqjpmedc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gexunychm.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gvrsakvmu.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gktusveef.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gfvthhacd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gpmtvmkrb.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gasmhbymr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gsiuzpwlr.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gwscsddnx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gauosjobb.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gtahoolka.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gqzqbanlo.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gmqzrbzql.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gzsdrkjsc.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gdmhejzyi.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gnwvjgiad.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gohhpgpgg.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/glblepmyy.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/ggexhsepj.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gdxnjlpqb.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gojmarigs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gspioymfu.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gxikjqybk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gipuwbvqs.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gfskrkmtv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gnwtovbzs.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gfcrjmccc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gaamxjpsh.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gzzggmpup.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/glrsnzmhp.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gwprauzyc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gegiqxrwp.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gpzppfkhz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gtdwvvwxy.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gaeprmupq.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gzynsjhwj.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gzhssxyka.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/ghmenuzcr.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/goazfwmmd.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/giobjwzjc.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gmcwxywzx.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/ggmyfoder.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/grehiprsf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gsauwkcdn.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gdzhwooza.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gmdiotrub.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gqaapoovq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gauefjgrx.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gslaaitio.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gaslcgfds.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gzpiqujuw.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gjzrumktg.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gkfxqusmm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/grleatqyf.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gxzxgxnnq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gkiztgfar.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gvmfcjcge.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gudiinyzo.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/grndiengr.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gpzewpxou.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gxyimqoob.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gfiwbnhnw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gzyvebkce.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/ghsucfjyn.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gqdxvbfks.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gumbzszst.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gyzreafye.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gvsjjplpb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gdvcykipz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gqqywyuve.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gqawzkjka.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gevvfcaxt.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gudyjzlsk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gozkqorvx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gdydwpboj.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gfnjvuutk.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gdievyyjp.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gayzagvza.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gqcqwfdvv.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gxvoambyn.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gslzqubgl.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gncrdurru.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gfksicqnf.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gcvmwodes.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gxsncrpkl.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/ghtlrfcuq.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/glntjklif.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/ghqunncnx.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gmzqugcqx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/ggfdmwfst.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gviidqbsg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gqwvtbvcw.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gehnpbrgh.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gjddubaqw.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gljaawwzj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gpokojeof.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gazsupfvb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/grtxdifur.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gvlqjoloj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gpqemrkme.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gntfokpab.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/grjlwomcz.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gjybgnzoa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gpciebazs.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gqqysjrvu.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gdjndfaxg.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gxowzsehg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gadxgimyq.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/guwuvbmyh.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gbijjbnwi.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gifkcefod.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gptwylqjq.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gfvjceeck.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gtuwdqyih.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gogxnqahb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gyspviwum.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gmqiytmmb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gwvikbull.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/grqxmdxaw.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gpzxdjxnv.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gtttefdgw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/glqacxsoj.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/guamdvfts.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/glzzahasi.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gwdbamccj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gevkjcvtv.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/grqjthtsv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gxlufuztx.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gubvcahsj.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gctdenqwb.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gdaucktvi.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gbixvaijm.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gitijuhex.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gcccokxir.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/goycthpdj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gsycingbq.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gzwvjbdgr.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gcoscavim.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gydtwheva.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/glpluxusn.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gnidmenwz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/glbtrhase.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/goizgemdu.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gaolwoyjj.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gpjkdasro.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gieemexen.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gvpafvlkk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gopitgume.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gfamtmfcb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/grfbatwgd.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gvmialulg.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gmbywohwo.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gzbicopnn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gspweeivp.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gnvnmrrgh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/glwpdrfoq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gmynurxol.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gnrvpvlld.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpqcyclud.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gadlqecox.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gevwtyqfa.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gtogtrpef.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gforbvzeu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gfkifaatj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gizzngujp.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gsccgaazc.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gnusnioit.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gaiypbwvu.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gxvifqvsc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gkzaudlba.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/grtdwngsu.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gowiaiyqz.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gcqbgeked.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gdzqfmpje.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gabztnbmr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gsyolmdtj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/glyumlvjs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gicjhtlvy.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gkmsytriy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gptdmkvev.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gdwdyjuku.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gyupptmwq.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gshqrnejb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/glbldaamf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gpcggewbf.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gxypsrpwo.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gywdrqyob.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gipygoibv.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gmzadnmis.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gvzgozjsk.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ggytthgyl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gobkgmocy.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gqiipwrrj.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gomazahzw.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gqxerzmqn.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gkoexkpef.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gptkxmkam.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gdeotdgph.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/ghzowtqnn.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/ggjdjawnu.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gslewspqa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gnskpckya.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gpebeyxum.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gujadamji.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gacwsgxtr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gfdrddpch.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gjmfiuctr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gzdfiqukl.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/grnsflqvk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gcecswrpj.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/giruuyrgd.sHtML


<!-- 参考信息 -->