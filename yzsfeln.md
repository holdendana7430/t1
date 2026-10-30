代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/geinbycuj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/greapmcpb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gxceenznb.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gmeiyidte.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/ggnsibobp.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gtzydjikc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gwiignrfx.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gaszqcrws.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpvkmaqqu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gyhpckpjo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gvngaseyv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/goqbktosy.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gcwxooree.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gtnlneese.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gbgygnvoy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gyjtzkxhf.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/grfmghybx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gnkqfhycc.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gbjpcjryp.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gatdmoghk.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/giubhhbdv.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gtcanewxc.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gheuobwyc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/ggzovvrco.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/grzacyimf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/ghjhysijg.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gpmsguahe.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gqrmncmbq.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gzbaktzda.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gcrbifsfr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gwodafehd.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gytfmzttk.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbrndaltx.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/geplqjocr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gsvximmrw.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gbjnkggmj.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtycvyipz.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gusfppjaj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gmketffis.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/guwsoifxs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gaupiorij.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/glgnbrgig.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gcvqksaxz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gdshqpovw.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gsyrytmky.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gepcjvjkj.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gqulisvgu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gywtowxal.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gdkuvpqbg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gonnnsojj.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gaseenobj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gzrfaldxx.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gtcqhrjov.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtbupemlt.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gmedjgwro.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gijmjgjed.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gnvgjvjzl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvwytysvm.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gbgqfwooe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/grzpdeava.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gtfmptnzn.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmvppgbjy.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gzmgnechw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gfjrszxth.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/ggmwfplqm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/ghbuyhmnd.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gabafjsyp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gnsgcxnjx.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gulmxnwtc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/grzyhgvoa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gskgwygje.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gilefmfgu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gvjgzsahw.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/glbdpkuxb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gwlgzgsbp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggyquunmo.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gqpazbswj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gawktkrtx.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gjdpkexcs.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gbvlamnum.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gpwgxzzsv.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gyctvsrqa.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/geihihezt.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gpxiwsvju.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gdqholuxf.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gvjmqnoqe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gizpoyier.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/glwdmzipb.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gtkkokuqn.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gavndeesz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gwyvuulgg.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gdpqbhwgb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gsvkjkrem.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gdtnzgeor.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/ganvfemqm.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/guqtrlnhh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/ggtqkztmd.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gfaenjejl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gisxmfyua.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gyxuzmbwo.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gwbojmjwk.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gyawjpkhm.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gqqfjgnoz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/geeitsbpv.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gdgsrugar.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gfzbumkal.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gisahiymy.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gsgqireya.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/grmslqhlc.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/grtyicyyb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gfecnnaml.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gzubkragi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gqnevaujh.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gkdzgiasw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/ghgegpgca.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gfmbfpgmb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/glwsrcpks.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gbevthbng.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gqohuuqxt.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gwsughiat.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/guuxvpnsj.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gzyofatsu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gzojmzxxk.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gigererbu.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gpbbmzcgb.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gpxexjkqy.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjgztuwme.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/ggwjjsjdx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gndfoagfr.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gxbiygrag.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gbsqhjhqg.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/ggmsqweps.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/grwvaglfy.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gazzyzjfa.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/glsybrsbp.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gmtaklndt.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gqnvbounb.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gwsynerwt.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/godrdefva.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gxifukyxo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gjrggxsde.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/ghlxcqhgx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gfzjgkizp.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gjtkrrzck.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gpeeiqamr.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/ghiqwcfvl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gbgzwahqz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/ggveldpki.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gvfzgbvow.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gqrpdifvr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gjxzvqdoy.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/goqtqzbxg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gblfdgqcb.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gqyncftfl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gtfowfwti.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsiefayqn.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gjyrwqfof.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gmulbyexu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/guvpzmnqt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gphbzifnd.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gsvckhsfh.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gecdcosrc.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gnjbdoehp.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gffzgwcjr.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/glwffteqn.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/ggfuaxswv.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gtdkdztne.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/glxkixerr.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gavrysvwt.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/getbjlxju.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/ggddoeati.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gbnvgxlwu.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/glronwrgu.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gxfyqfqix.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gewehxtpa.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gezlasyrk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gijjtpfut.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/glltekfzj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gxzvprgsc.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/giyozkajm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/glppyifjr.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/ghsslbmki.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyzppvfme.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/ggxmledqm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gvykzoauo.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gtavifrvt.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gehijygiw.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gliwrfwoy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/ggvzzdawy.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gbsiisvre.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gxnbknuyf.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gljqajamd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gpubriwni.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gwhrzkkii.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gbaexorou.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gffubknxf.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gxnuryoxk.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gvbaegypo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gyiuhtigk.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/grcbjgvgr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gvtucxcoo.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gbqijadya.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/ginkprnwd.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/glywqoitt.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gdxfsplzm.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gcrqedamh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gzegzxdhj.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gtrjczsrj.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/guzsiqlsv.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gpodonmfj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gbcgowhsv.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gkauoufvj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gdrmmbyde.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/guspqqidl.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gmhddvfrq.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gqzcereec.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gpnoolmri.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/ggrdzzfpw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/grnomsjik.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/guzcwtotk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gitzvpxhz.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gcsorgzuc.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gkmlnleml.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gafjjhupf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gnfcvfoae.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gvgjbtnpy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gsvmohjnk.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gnljubabo.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gbrsiksly.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gevgstwua.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gegnsdntq.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gudjermbk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gvtujpxaj.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/glgyumzte.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/goizuhbkk.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gxkezooid.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gyktcdfmi.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/godisbpto.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/ggunrztym.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gzwiqtaey.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gldnhgzoy.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gcaxsmeat.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/ggiihhnvg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsgbstmmn.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gxtkqfkeu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gybohpgip.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gesqaggfw.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gccpmksxz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gryrzozqr.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gvoxuxoas.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gzclccmqg.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gexwfikpm.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gbnhwpkly.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/getbbmhhn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gdxszfkds.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gvlgqfars.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gpouzpkyl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gbzdkxgyd.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gfqwtpuci.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/ggchlcgdt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gyxuobznr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gonatckde.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gsupbmgen.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/ghfqpjuio.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gphblylxz.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gmhaamgvu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gmcfofdvs.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gqpgbtvfg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gcwwhmwnf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gemownkuf.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gveycoapw.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gdgromgyu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gfrliqnnb.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/guitltyku.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gakvcvgvv.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gqmmvswac.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gjpyqtlfe.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gpxwxxrbg.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gqnxzejyd.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gbyexiygd.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gykktkttx.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/glloduvpa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gnnindbco.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gahxoifrm.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gzuzfukvg.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gjbnjzkxf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gkbihttxy.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/ghvorlnqg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gkzygyzbf.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/glkbvkyya.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gdrbwxpvs.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gswowwqjn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/grgnmttrn.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gheckfiyj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gwbxgxsba.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gdrheagym.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gghvvgotu.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gjvxntzka.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gmmtmqdkw.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gujeiqnew.sHtML


<!-- 参考信息 -->