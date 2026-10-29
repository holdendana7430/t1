代发 wailian999

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gprhvqnbr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gmtqifxra.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gdoxbddmp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gmymblxvx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gmehlacoc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gzkxbzzvc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggmzrazze.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gatqattig.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gqstdepwc.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gwjybumwc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gfeyoavrj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyhasjjyy.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/ggzwocbdi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmgryunif.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gohcavjry.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gwruipuko.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gjtmbckwl.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/glemtjqaw.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/ghaxysttm.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gxiocngju.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/ghubytooz.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gmepgkmet.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gjtwcvsmj.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/grsedxmru.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gouhncpnb.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gwvpauald.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gaajrsonu.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gubbqascm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gbodcfrdf.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/golfntsdy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gwvephupn.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gjlvoykzs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gpqpbfdqk.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/grnhaqnln.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/ghpjexeve.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gkrhwnexi.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gzciukpvm.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gargbkenm.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/ghfumlqab.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gmkecmogi.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gjnfmvzzz.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gxcoxgfny.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gpqvefqsw.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gbhuboffc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gkzqpmovl.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gqzbjsnmf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gaemdsrqm.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gqcrmbtec.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/guwnzbqzt.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gtwnzovuu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gryvsijng.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gksuirmfy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gjimjpkef.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/glkpzznqv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gibsjsdsw.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gsrklufoe.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gotguunyx.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gtmevtbiz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gwfpjjzjj.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/girrzuksy.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gnstukkjy.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gmadoxsxq.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gkoksckrl.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmyoxklgs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/glnfcwwir.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ggiymhmcu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gfntyyiun.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gyyzbogzg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gzfqaayij.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gchbugwwy.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gfjtbzbqw.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gwtkudsfx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gwbuizbdi.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gitzjovmy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gqycezyiw.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gcfltkpoa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gvzkomdwr.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gvagxqwnp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/ghhmiaegl.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gtsbagwym.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gxddmmfwo.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gnqvvvhpj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gaquymkza.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gnerzkhau.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gjnjqsthi.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gerhokvad.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gknedcish.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gopdnyycm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gkoewhlxc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gvgrshhkq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gsbxsltzn.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/ghhqgtxfc.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gcjpvflop.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gogepnuzm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gczkwolhb.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gsgqnsrco.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gdvfgpgdj.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gxklsatir.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gaqrtvaju.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/ghyrmworo.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gbzxagnrs.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gzkerftzl.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gnkwqupsk.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gcydlprmv.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gzgntabts.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/ghgorgkts.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gnxzfnujf.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gcdmuzeqk.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gzkwknlzy.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gisesoidv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gggbnmdys.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gcegcncgp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/ggovhtenh.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gkezelxyb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/giujrqobe.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/glcweldjk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gtscrivvo.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gzwaclfri.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gvoqwjnoq.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gcclmacjb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gkkdfvcvu.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gxrankueh.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxgvmclba.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gmphlpzmb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gmzquiyng.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gmeoeyiqn.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gsdlyxhqa.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gfrildcai.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/glmygurpo.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gyhseufdx.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gwkdyjcqw.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/ghhkefofl.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gueaapwum.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gpvyatthh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gnjrbathl.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gzbmirnyv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gmxwclnaa.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gcxhwufdk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gyfuiesly.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gfifsqyim.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gbgomepdw.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/ghgwmvzmz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/goudzzjbc.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gfwphjddr.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gfakwzrpg.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/ghircibzn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/guaaamoud.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gslnqhoay.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/grhkspyyt.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/glhjhkaql.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gbkhwvcpe.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gnamkskaw.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gwenxmyxa.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gxpujkbsz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gfmyzzwrx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gazlanlnh.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gqrezxzkg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gxnqfopdx.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gnjxzkrhq.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gijqsgxmf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/glblablmh.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gvzyonhdy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gbcinusdc.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gutaexmsm.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/guslpwcuj.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gjtzvoppg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gfmbnrxhv.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gmxeigruw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/goubkpong.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gzumuucuz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gytdwpyzn.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gewuhyxja.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gwkxqjvzz.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gjuyzhata.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gbnsafqrk.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/ghepzisfc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gvtzlajvv.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gxmmydxhg.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/guqgtflol.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/golwuqcjr.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gkqvmbggv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggbcjusgo.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gkjqycptz.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gzukcvfna.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gfvphxxjj.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gbgdtxrzu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gwjkpnydx.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/giboktcoc.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gnsksplgm.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gpqgoymaz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gxelokkcs.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gqffxxgbb.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gxnlmkvab.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gwlouybwu.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gyisdcupc.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gnhmegcol.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gdmebnouv.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gpyxnrnnw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gmsnuxaft.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gkobooelt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gntcswlgo.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/giefvzdqa.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gmahygyyj.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gkhjzysdj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gsbwxsftw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gerigeluf.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gzuxxzetb.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gxwauvefv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gfzyecivn.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gvrcmtvxe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gnnyegzdv.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gluumojzl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/glyvtilzc.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gjefsioqa.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gtcrmmpoc.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gokqkpiyw.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gmytdivkx.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gnldkpwuw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gxjjpblzo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gbnvtauzc.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/glhrcsrcp.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gjejydprg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gzlxrsgjk.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gdgzosfgu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gfjnuqpum.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gicxotxta.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gvqutxhai.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gogqtbutk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gpukzowwb.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gxcqdxgbz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gjnuualsz.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gfqidoecz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gjbexlsmu.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gubkatdqf.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gpofpjets.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gkwyoyzgg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gkestyhfh.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/glhtivlax.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gmhbupfjv.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gdsjzqvyj.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gnfoerfch.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gkodzuyqv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gxregltcv.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gbctjebhv.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/ghjwtqcez.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/ghlpqmuco.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gdxhqdgtn.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gidawqcpv.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gkcsnawgc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/grzpsuvft.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gbkmvovoj.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gkqizgdwv.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/ghhjtzvay.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gohxnlcvi.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gtvzsrvjg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gcnpmwlyh.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gggbukbvc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gzdyetsuf.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/ggcppcama.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gqtycwlpm.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/geqogxugi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gedkmgzaw.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gqbqunsrv.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gfueheygh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gcdnifbxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gmafncijp.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gmqxvclcz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gcehttihk.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gylbxduey.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gygeydxwa.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gjxhavvzl.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/ghvrajfkv.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gpucpchmc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/giupvmekk.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gdomnwlpw.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gpezaahan.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/glxutusya.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gearesqlu.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gchuqkwdi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gwzcrwvim.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gsctkunci.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gosttwzbn.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gzzsovbnd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gdywpsidt.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gphlnofxu.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/grcsemvea.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/ghvdykbfx.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gydcnpvvt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gedukrjqz.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gwwusdaqk.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/ghxzisaxi.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gokemdzem.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gndsweull.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gcgatmzbh.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gtxeczayt.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gvklkginc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gudvpbmkw.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gpilikexk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ggukiewsr.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gkirnpzms.sHtML


<!-- 参考信息 -->