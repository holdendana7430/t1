代发 wailian999

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/glvrinwbg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gccwnkubq.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjlewdot.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gltcltiln.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkzmgokw.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdwfkhvp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrfisfii.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gfoaiarpt.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gehkcwxdz.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gvasescqq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gmdeaspon.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/ghqdyttdc.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlypblej.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gbivnypbh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gwzxvcagk.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gizzszomy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjnhuovd.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gdmzrhppf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gytjtqzah.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gwhbwjequ.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gtgqbhqfx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjtkikmn.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjrmqayl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/ggvtjjtfn.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/glmapbyim.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemaniavv.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/glsvaghol.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoyfzhkv.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/glzgdppef.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnvkernf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjgnloyb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdvenctar.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqdaineo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjpremuf.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvqygjpm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giixvazkt.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/glomuxgog.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdagucvnr.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gxreubpzt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gloqyhmig.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrpriofq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gcxjwzojc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrgmwsps.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwifhjmid.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedbblbcq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gededqvdp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdcdwlxe.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/guvkchhgz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpltmeinc.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gzbchghyl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gzsxqlpza.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpbxaqkr.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gbmbommbq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gioqnbpju.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gseriddyp.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gugqnwawe.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gpwtzxdog.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/grzhnxasd.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gsuikdzxc.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/godiyzymq.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gugvlabit.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwluzumxn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgrwgpuw.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gvwsguuyw.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gevfcknvj.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gtkrmgqnl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpydkaaau.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcqwcimkc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gyetvwgkq.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxuzxqnx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzslyfetn.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlawrihj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiqkmuyp.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gsnubriwj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxlrireg.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfknjobdy.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/geymxkkpb.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gmnclegsr.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzvptmfc.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/grodhfwar.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gxngkusye.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/glczfeemz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/grmrvsmtt.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxbwhemd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghwntxiqm.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/galmvnmrf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvofasuc.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gasntngul.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzppkpaeg.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gthmowvfz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkhvjjrpz.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gueoxnskl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gowctlhyd.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gzwxcoolm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghrqsfkvs.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gotugwphw.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghalvwszo.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gpamqqwuk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwfjajqva.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gduyohzyx.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/glylmnscw.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/glscrjpye.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqqwxynp.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbsjmwibb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlbvxmbl.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gjvzgqfyw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsetsoek.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gbrkopuah.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqiujavwq.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gezotejsm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrkihnsk.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjiggdvy.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncjsuntg.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxznudjl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwbljmgv.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gesproxyb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/girfgubsw.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gpomozagi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/guzygcdyh.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvtbinbbn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxdzvsao.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gtxdlzhjb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gicgivpwt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmmpepgz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwkcrauj.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnvvmghi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gffqcafvu.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfbbecqr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gysqrpehr.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhvcdglh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gjcjrlahc.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqdobpjt.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/grrznhkop.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyjgttnd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyomthnaz.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gpsrjzfmv.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuhbilnj.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhpvkdcm.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/ggkkkqgcr.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gnxsvpgqh.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjnvsqng.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gptddqikh.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlbqmvyb.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/grjuvxljm.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkrjgcco.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gkwiylzrd.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gcgmbedtk.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfngbobi.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbxkcrog.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/ggepamanr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gjalvrydz.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbwzhuwwa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggaksofnl.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwonsivin.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqhxoyru.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnrrlkty.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/ghsddzvje.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gskuixtfh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmghrsgfh.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gxobzrnlr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gdlikaxsm.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmsrycjp.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjsmukbx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/guekioati.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gftcxxufq.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxogjjiym.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqqdestfk.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfyhyqpp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvogghcw.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrnluloh.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gjenicgfz.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbamrlbv.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gqscxgvhl.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxidecxfm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gdellhtga.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqdsgeom.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gpedsxuft.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gmlaoqehe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gtykfezlw.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/glantqnhx.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaxbshhj.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhigcoru.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbepmqer.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gaedmkuao.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqhhfxhf.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxwqipgf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvahlnluo.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gihdrkrip.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gtaxgtzqp.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gkrtaefpg.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gmgrlunoa.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/galkwqrpo.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gzegcygai.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqywcciev.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkufxntfc.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/guckdljrm.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrdubujc.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gopjxafup.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gfpuacusy.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gydejmthg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/guqgtetis.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmwmlusu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgnlmoao.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkuivcvu.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gbskzhrxr.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gttydpmhn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnrziaabt.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjossbkj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gbnvwhkgj.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfmpwwlzo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/genenbzwr.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixyjetso.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gplaliufd.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/guqwvcfxw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpzntiiil.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxjqnhrj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdmutylg.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gakejxwmj.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsahvypmd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghhdjjzwd.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/goctcpwuc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmweettn.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqkbmltk.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuryfljy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grsvfkbil.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gyupexxdw.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gcgnxgtch.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbcnfwbd.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gobubhdyc.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gnawpwkth.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gezvbjlhl.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gdahyvhlf.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghklxbvsl.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gqwdqnwzf.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gvuqhjzrx.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gtedqfsqs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gllssjeqm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvbtermn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gujrkhiux.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtxuktxp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcrruwse.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gysazuncc.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzmppjaq.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmeblrxcf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gnhhernnz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnznuxbbq.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdafojhq.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtxvduvez.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggerhfguo.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwxwykcz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gowrshpli.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gvbhugzrs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gkirlfvow.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiksmpje.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gfofyfpdt.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrjnplpi.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/guanvlino.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gntdiflel.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gweueyqun.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/geqccwbno.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/giwmqmoxx.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/glgpncbhg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdngwfrxq.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/ginusevzb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkojuebjf.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gazhhbxsc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwaahpjy.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gtfddwbws.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gelapsqje.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxibfgawc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/ghwoojxxd.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxuyfzam.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gqnskesmj.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grphxnylp.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gnfhdvduo.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxxmxkaa.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gqdpbtiye.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gtflblcyx.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcynkpew.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpjvmwncm.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwmkdhde.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiqbhftc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmgrdaff.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjxxzfxs.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gbhybnnos.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/grtnycgiq.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gsirmyzfr.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqoyymtxx.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvupkqjg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gssyejinb.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gswsfinmi.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmkwllgd.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gxoxanynw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhqfsjiu.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjyswnea.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxihiljud.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gqwvtuoed.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grsjdaxdb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdzvqwjz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/guqcmreuo.sHtML


<!-- 参考信息 -->