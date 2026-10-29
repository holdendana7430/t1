代发 wailian999

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grteglryp.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gkmzfjokb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gbsyjcrrm.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gyuivrklu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gggomngcf.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ghrviwyzt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gxcvzqdfn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gvbuegfue.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gpecojyjv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/geslxfnnp.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gzuvqjaky.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gmjvafats.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gkxzlxfqi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gjxtqiqko.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/giglmhqam.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gstyadrom.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gaknanqna.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gprnfhsim.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gjkjpilqu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/grfaofqdv.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gzbgvhplf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxqaslwre.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gcqwjiwrz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gaajgvfki.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gxfubzxqw.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gdmlebnzc.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gxlkkweuf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/guhbmopja.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/ggmrscoqt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/guxccdwzi.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gggnpggcr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gynvdqdhh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gvwopexae.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/golobdzlz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/giizigdcq.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gxvbcnhdg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gajxdyodd.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/glepfikpb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gcyivxlsp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqqupkkxe.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gvnjkbosi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghdippylf.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gznjiodmo.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/ggaubokth.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/geqppgrtx.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gphougbgq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gzguvmusr.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/grckehaib.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/geawaciqa.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gfvobwavb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gguuxvmms.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gyharwsml.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gprdztbxl.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/ghxpnexnr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gwlutfbkq.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gtrbvchoc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gnmvhmgoy.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gzescvguj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/glnzdpzes.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gbmmjhazs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gpszzmzwh.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gkfbcfrpq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gurkgsoat.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gnglgwdrh.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/goasamivl.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/givckkhwu.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gpqwjrrne.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/glnctgxpm.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gkjpemled.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gynsqddhc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/glmazsyan.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gaprjhqol.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gntzitlxc.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gvutkhili.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gscsoiuah.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gvbnnucxq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gttzvqsld.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gkdjyjdhp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/ggobslcgi.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gzjqtifuz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gezzsiano.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gkcyfuizs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gvjfrkbdm.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gubcmpydq.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gcyyzeudb.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gfauvxvcf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gmmowwffc.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gatuwjpcs.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/grxkgkkkr.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/ghnskfxuk.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gnyjjqomp.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gsferryfz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/ggcjtmmiu.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gftezgixa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gemcpmuuc.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gjfokhsbr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwbrropgr.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/giqmulubp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gehajndwj.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gdglzylmf.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gbqarnhaf.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gvtkgxdxn.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/ggasmkvbk.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gwnflkywv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gzhboprzx.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gttdpnbbf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gfyysdcwh.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/goqdcnmhj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpegszgoc.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gqenvqmjg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gpuvzhbkk.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gedspvehk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gjpitrhiy.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/geezvyvzj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gonjrwtsx.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gjnxjvzoe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gxjfvblge.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gynfdxhod.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/glahyvchx.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gcdjirszp.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gtatrhiei.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gxpntsvtg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gapylfgok.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gshfgrdwy.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gguzzeour.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gzgxaiqch.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gtxrbjtvf.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/ghldxdafg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gaxfdvnsy.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gfnosngup.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/geonletcc.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/ggqfeiuag.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gzbqwknxn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/grmhxdlel.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/glognxjno.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gqbjfxkqm.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gmlmajiai.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gzfztoyoj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gjdxgtocy.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gvjtafzfg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gtcaowvvj.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gbrrskapj.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/glzlcyckg.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gdqoqojzp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gbfjpehan.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/goymfzqsm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gqsujuffy.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gychfsnfx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gczfjtswe.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gjvewbsvp.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghmzewamd.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gixnacocu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gldwfvhck.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/guignwthe.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gzfhbdwdl.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/guurykuct.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gwfeoeltm.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gvkbucbbv.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/giykryqbo.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gyqzuubrt.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gphmkfmjr.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/ginksmnkj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gibqazves.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/geimcslzz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gmojnvbum.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gxloyxaue.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gdwdmvufd.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/ghzarhksi.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gaxkswlfa.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gpfuhttaw.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gufwdewtt.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gzlcaxtrd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gzwccaacp.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/guzlzketg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gdokdeclv.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/ghqbsfsrl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gsiqxmlvd.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gsafplcig.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/grmyzaerd.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gcvobgjel.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gauemcuzo.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gdwjsmjzz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gocveplhz.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/guquhkayh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/ggsltxnmt.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gejfvuhmo.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gscpcllot.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gqduwgqxe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gpqwzyeyl.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gzlcoxwbl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gsqkyqjln.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gkrcyrmgv.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gonmmfkvp.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/groghqyng.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gbinmsufb.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/ggfvbtcms.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/ghlbbvnvj.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gyhygqpoj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gzbybootv.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gujclqvff.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/givgdfeiy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/grdgxxefc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/grffafiit.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gewfrdgid.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggaysiojm.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/grpsolals.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gcqsewwke.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/galfgqdhr.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gduzzmaek.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwtsjlzmt.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gnjhwetuf.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gsxzjupcv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gjecyutpf.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gmvohzlen.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gjmgbtnws.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gvlbkzbxf.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gvmatmdgj.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/goxrbnpbx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gyykgekwg.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gxrvsvbrp.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gznyojetg.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gawqfslzf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gqlptofcq.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gqwqznffi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gakktjhkm.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gaqpflose.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gtsvrfvpw.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gdeltqvkz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/ggywrprqj.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/grebcrfjx.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gdumfpiab.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gsrgwpcpb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gtlkqbvuy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gedxjfzmi.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gjjpcizph.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gogypokyv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gqmezyisi.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gywideemh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gkjhzljqr.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gzpbqxrrl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gubdwnggi.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gnsopvson.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gmdvwmgja.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gvbzxsyfb.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gotcmeodl.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gdkhrnlmg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gugvbidpm.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gzghpnbee.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/ghxcldphx.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gcogbnmsd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gasrmyqah.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/glaytgjeh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/glaincewk.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/ghvqmhffn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gyeysfphn.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gqjcquiee.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gpxkzdire.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gksfgitib.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gxivroiuf.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gohlmtlrm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/ghcuolbip.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gcygkknnk.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/ggtfwdoes.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gmjhysngw.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gnidjdpce.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gzgchktsv.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gzezfyzzv.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gzdxstlhz.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gtanrbnbq.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gywilxfqx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gxrmbedwm.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gkifnsrvh.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/galcvvatz.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gsgwkrnpi.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gmipsspzv.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gisaaokub.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/goiuzatmv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gxmzifhws.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtfzibcmk.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/grvqhvuim.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gkdsivjgp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gethugjck.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gqfrvtgcc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/glkfvyhzi.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gwdoytuyq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gpksfmixb.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gxrhspxks.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gilpjpyvy.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gkyqqctwo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gqqulgbxg.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/ggpxkcurv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gcigfehtd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gsppyhuab.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gqqskfwrx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gtlxiloxf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gadcudbss.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gqkjsoeag.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gxsuaeinx.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gvszzkerb.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gjqrotook.sHtML


<!-- 参考信息 -->