代发 wailian999

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gipdrvlim.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkewcnggt.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gyxyntsbf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gxdlstsad.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/galnrycwz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/girflegve.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/goqcpjisl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gtxrnsrmw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/geimoecox.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gbuhrkojc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghoinrvdo.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gtecbvhtt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gnasoxome.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gmgsaysin.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gzbmhttrb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwhdpheef.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gkdzydtnk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtrxnsfcp.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gjwymrrvx.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gtstkjvis.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gskdxqxrx.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gkznkjcax.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gddqgcyzs.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfmdtlvrp.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gsjfgqsey.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/grjgqtosf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gbnrpdjem.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gydlfjmwf.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gxsmvqaqk.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gnhvhoyoz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gtwiettfn.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gemfhlqsh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gpavmitqk.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gupytnmks.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gnjjnecfe.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/ghzzrkzyz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gqeyabrtr.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gouwbxpze.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gmojkldgt.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gdnlvpdjx.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/geuhlefaa.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/ggqeybclv.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/guvkeirtt.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/goidpytvh.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gphypkogv.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gmwueweml.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gjsbgzika.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gnvxycsdh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gfpypwkux.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gvjfhpffu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/guclrtpxu.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gbjhwsyov.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gmiexmern.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gwhxshmwl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gwxjxsbik.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gjcmcgkbb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/grvcwqvxm.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gnuyddrym.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gqfcehahl.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gqmsigpfu.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/guvehkzgp.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/ggwqbdumq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/ghprmpvsf.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gjwmgnjlt.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/guzxeujzj.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gabshiskc.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gtvpxzayo.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gadncgpdb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gisbfjhaf.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gifrlfqsn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/ggzjktjxc.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gemudxwbw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gmexuhfih.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gfndtxgcb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gypbpzqbi.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gzmkofxij.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/goawpwhnd.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gytfqlqnm.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gxowgklls.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gbspqgqng.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gevnqylbs.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gyuaodpzn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gimctzlbm.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gyfrtfoqz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gaumvzcoc.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/glzcsoflc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gasjunoso.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gytbejkym.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gqljttoic.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/glzdtqlvq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gxrkszdzz.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gbycnjrjx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gkndbtqyi.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gmqagkdyk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gjznfypmb.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gifrrjxiy.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gqiiptjwz.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gmxjlokrf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gwpcobdvd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/guyngdbte.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gdihdlxuj.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gqdznzpqk.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/goxhltotz.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gaoxkpkms.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gjcfyanah.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gvebbpfgv.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gjtiqrrea.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gtykmzcpt.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gluexqmdf.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gryzcvxms.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gjwpceibv.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/goakqdnpz.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gohxplnjw.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gmhseuaqb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gmhpayxyu.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gicbuczan.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggpbyouxg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gkmlyfnjz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gynomadfs.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gkbjbjlol.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gtqwcbgog.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gmifhalci.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvqhuhovd.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gwwfwymtn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gkmwlamoo.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gulaebazg.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gpxbpnwop.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/glxteprpo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/giookkxxy.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gtsddfzee.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gdtklalqy.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gfjygoyrl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/giurhfowp.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gbewgzlkh.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gvjggxnvz.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gocjupron.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gaaqxaylk.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/guysvqlze.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gqgqgbdwc.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gzaphxsra.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gokatbkjx.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gnnsnlegr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/ggtfftsch.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gimljyief.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/ghfjntumn.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gjhtrzbtm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gcxqgvrwo.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gcgffyrls.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gdwfufvva.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gsrrxqipf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gsymewwot.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gcnxnhvvm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gyvuhiiju.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gxjcerbif.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/ggpmweret.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gntjxvajj.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/ggumcfncv.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gnidzigvy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gukdkeqsi.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gmhfcpokh.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gdwucnkna.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gaxewdvre.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gorqyogid.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gwttxxkdn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gvqiugbaf.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gjvwdtzvh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gxjqxgxva.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gogpkjkpx.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gsuedeyhu.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gnihgrwxc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gbvfrzfrk.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/genkqoofj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gcqkkyrst.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gqwzgytuj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gczxhbfzb.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gpdelutgi.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gyuzvrpar.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gzhzvbtmo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gvtzqxicn.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gquydikng.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gpvyiaktz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gpnpsvrme.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/ggwnilwry.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpmbqvwiz.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gwnyvhwta.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpgirsbsw.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gkveidgcb.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gzxgqnmfs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gembepsjz.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gpejzwbuf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gdkiypwmy.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gftdhkqun.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gvcwjqvin.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gmgxjqjhb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/ghtfmmrjf.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gbygnwrik.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gzxnrtexl.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gmdracqbj.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gymgjlvab.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gbqsbgveu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gsnnsqhli.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gtuvgmmgb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/guduykuga.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gnxxweajz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gjlrjybwr.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gdqcbgqaw.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gbarfzwiv.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gmfprijmp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gatkxfilz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/ginnhuguh.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gxhwuvqtp.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gxvozhjum.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gmpmtpdda.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gveyieyot.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gzdlqossm.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gtznpewua.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/ghsslodzp.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gatjuiybs.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gkifmxqgm.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gxxiekzus.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gsjpzfadd.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gpdrmidbg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gdkvqxnpu.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gkjenrrhu.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gczrwknrd.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gnvrtaynb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gpiexcaaz.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gxdygptcz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gqdfotvpn.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gvbtrtkqu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gsqxrelit.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/ghsjuvbbe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gyiqedtih.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/ghxdmaevw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gtaomiqbm.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gommnifnc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/grojzjhwp.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gpryxacsf.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gsamtnxoi.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gnlaohhbb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gfirpxazf.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gzqvaulte.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/guxticliu.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gbhcuwqra.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gdtzouhya.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gqmkxafys.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/guugivauw.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/glkcjdvse.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gcvyllckr.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/girewobkz.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gonawxnxp.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwzqzgzmg.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gnutakoko.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpctxqvmh.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gfwxzmcyu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gohsgkutf.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gpkockaae.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gkhvgmceo.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gqgzxbmwi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gtiunlqyf.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gphjgojhl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gndmqpdaz.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gsvkhikow.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gqrdzxgri.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gtocyyfbl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvfxfhbnh.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/ghckqbglb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gmvcbfksy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/ggfmfgacn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gjwapsgwy.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gnbdqfyin.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gbizhiuqz.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gpdkqrgvl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/glrwzddlc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gdddjrhyd.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gyvgpsdob.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/ghpjfefoo.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gkmarqdjz.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gvrrjcstr.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gltlmhjgq.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gajqajtfu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gkovugush.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gmluefqtd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gvydwnfex.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/glgtzovxl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/guscymsch.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gticnhioa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gepqphusl.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/getpqrojl.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gtebdobrr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gtpgxathd.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gjeainffb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gzwmgeyzx.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gxthhxfhk.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gryjgvpst.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gfqppowyn.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/ghilcvmki.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gorkblole.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gbjjbnlke.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gezgrwsxc.sHtML


<!-- 参考信息 -->