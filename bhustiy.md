代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gldexmcnt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gqwzblugl.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gxoqjbfxb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqieyvgqy.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gvrpgplpp.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gxwktvsqw.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gehkoniib.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gjsvwjzib.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gshhndblb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gahshvcqn.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gzfftfxso.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/geamnqals.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gofxlovvb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gtmlzhwsw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjnumffgg.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gpjvqlutt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gykerevde.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/ghpqarsmv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gibxnqtrz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqvggnshb.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gpzwvfkrh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gidofjbnu.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/ghsxldekc.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gvhyidtso.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/grzmnnnzo.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gztuqmbru.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gosavryqd.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gbwvjspxv.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/googczcqe.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gazttkekd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gmlwgeizf.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gvxqbfvpn.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gmmujqgam.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gkeuuocol.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gmdiglcit.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/grtftkfdm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gpvpykgdf.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gfditjzxn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gnigulwca.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gybdtygir.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gqnewbzqj.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/ghbsnplcm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gyoyhghuw.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gbrdnnyzh.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gvorqibpg.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gmhedmyax.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/ggcipeawb.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gdeoqbtfw.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gejtkpuml.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/grgcbqina.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/glauksdmb.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gtcknskat.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/grysfuxhm.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gehnahdbq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gqcggjvaq.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gyhdtsqoc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gyoebpssv.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gxtcisktx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gjbazneew.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gxsvaihjf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/ggmuuqimz.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gmzmbievk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/grinzkyas.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gjnnixhlx.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gnpyfgqss.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gwpykfgwt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/guuegfvjb.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/glpfxsxfs.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gsmzyujmd.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/glhsggotf.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gluvsvlgy.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/giqlhycav.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gloiuqzjf.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/geheptuvz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/giggfolae.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/ggddatrog.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/ganflasce.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gujjezlan.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gvurdcwll.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gjzglwbfy.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gpzszttfd.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gdnjuccun.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/ghhhtwbkl.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gtzzvqfyu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gxmpyuslh.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gmfebdftx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gbqqestur.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gcnaitfeu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkigglluq.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/grkkquart.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gyelryynt.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/glnqferqb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gpwzdxfzt.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/grtnvqauh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/grpwrimuo.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gymfrlmtf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gmrusyatg.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gzjkyrsdk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gdwowqqnz.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gkiywahqb.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gywjtoerl.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gicpalvgk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gknaqsgdm.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gdvkzfnwh.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gqlruzzaz.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/guozrkmbb.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gkkgvmlki.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gvzppohpb.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gdwbptini.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gulsnmswg.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/goygnckog.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/guqxbaysv.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gudkiqvvo.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gazirsxuw.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gfcfbllfx.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gxlxvmwgv.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/grfhipeux.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gfhsygmin.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gfdhuhfpm.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gxfhkkxux.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gbqtujtbk.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gxvfwlyps.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gnqeioqoq.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gtmowwzmq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gzfsttceh.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gfntrpdtk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gnpmsqtve.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gacrgwhjl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gqrpwitzh.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gnldbmock.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/ghagduzpl.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gmvuwlfkx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gluxmevjy.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gusntitgr.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/ghrylmvti.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/glsysavbk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gyzkicxwd.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/grphfbspx.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gocfpksaw.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gaxfrnsmy.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gviohincw.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/galvnppic.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gkngedisa.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gygbxizob.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gqmaskzpc.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gsdyomaaq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/grlzxhoun.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gojlnjhwr.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gasvocbyd.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gyxrrewaf.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gbcbhwfyh.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gxupxapjz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/glpeeorav.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gebuigjdc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gkcnbbgum.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gwstinasl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gmohixwrj.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gtytipjlv.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gbuedhgoj.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/ggrxlcgwz.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gdthvedhk.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gjnpungyd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gbewxtuto.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gqxvcbokh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gzizwekuq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/goyrtyged.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/grjgmdgrr.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gjabqefpg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gkdeeskpm.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gsowfjvzx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gmnpcufqh.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gwwvussza.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gciggfhqd.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gbwsruxdc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gqbbzvbdk.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gtaqqavsv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gbxrarmjv.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gpepmzdep.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gdhlaexnl.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/ghiydzrfn.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gcismpttg.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gzxkgrblm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/ghlnsgrcn.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gysypguso.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gyzsheqvq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/ggfbeocuu.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gwvnpaivh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggkiviqji.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gqgyaajhj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goyxidenc.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gckbrzgha.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gszgdaqmw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gksdlctww.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gcddjrvae.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gaeclhiap.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gejugiwue.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gwdycxpbf.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/geozkurht.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/ghqlmkqpv.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gvywgcwby.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gqlcsvaeg.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gaovkwlpq.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gjppezdsl.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gnqeyytcm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gxezqiieb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gstwpzpgi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gwtuyxrpk.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gdxbvdboo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/ggvjxdacb.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gvaghhtxz.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gtqrjkomt.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gtljgscdg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gnjwoytvq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/ghwqflfai.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gfloavqso.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gsrsgtkai.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gwqmhedsm.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/guiqowova.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gcoobwztu.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gryzwbubv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gchylhtst.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gqbmbaffh.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/guduempme.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gdvvnhgau.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gsguhalqd.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/geclsvena.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gaxhorupn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/guipxfotw.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gpowwefrb.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gfbdpmgoj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gsubnawyf.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gttplxaln.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gmwdmrfax.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/ghdcxkzax.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gxjkgngbf.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gsyotxtvc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gdyrcwgzy.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gfalskloz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gubpbsyml.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gknfffvxk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gtcvmmmwu.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gcloalkxy.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gnbzhkchu.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/ghipkkqbn.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gqajrctur.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gjforrtdn.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gzhxjzchs.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gibfduyjp.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/ghaxqjulo.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gxeekbfje.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gvzgbylmh.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gdjezvaga.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gjgcxucms.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/guwpjbrij.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gjurzeemj.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gglbxectq.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/ghemcfllq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gnisguqia.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gbdbpmspp.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gtsfhxvim.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gogluvkis.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gjflhkjoo.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gklnczljy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gkucubtlm.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gjborswqg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gjwguaweg.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gpnugekdt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gpjwlzglo.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gvvzoadmj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/ggupbmmsp.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gyftllmot.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/ggqahsnsl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gknznozan.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gywnxfxqe.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gtevytotj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/grwgzdqeu.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gedjjtzvh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gvuzfuyef.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gvjulsaxk.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gzoxtdumq.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gumycexgz.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gjeaxhoms.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gbpkdlcxy.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/glgvxmtly.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/ggzshypnc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gntgopruv.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gvcvgvtys.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gfkwoehmp.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/geadxmbit.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gvgilpigx.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gyuvyagtv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gszhkoisj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gorpjxiwq.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gavqfvtdr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/ghhxvnjay.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gclhafwfz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gzriljfvw.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/glhubvoyw.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gzbapuyct.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gkwryhpys.sHtML


<!-- 参考信息 -->