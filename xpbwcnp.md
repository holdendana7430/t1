代发 wailian999

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gyvhkaycm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gbzlvzgbh.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/guhwqjalf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gjjmnwiim.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gjutpvufn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/glthdunxv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghroahpdd.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gwgpmpjub.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/ghuxcbuuo.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/grnntjxtn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gahcdoxst.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfynkelyw.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gvelujcmm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqphwhkbo.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/glliczevb.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gwtaoriju.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gftdkmcxw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gcmawrvui.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gzopmegos.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gnpsothyn.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/garoqzokw.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gwpflpeto.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gnygqevih.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gbupavrjl.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gmcpmmsce.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/grfwaczxy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/geantukvk.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gibckfksb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gjzchrunm.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gmuoiizbh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gidogghet.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gawfktcml.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gmgntjdsj.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gvoefcweq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/ghsybvpej.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gxbvfssgl.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gqqzdrslv.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/ggpwrqkhp.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/geehxmott.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gnvrmdcns.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gzowpksmi.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gzrljlrzw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gcbqhydwt.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/grvtnmort.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gprxdxiqi.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gtfqvhvak.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gzmcqgmxs.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gbulgctbv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gvsilcifb.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gsdcyeqqn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gqefqjday.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/goyptcjpf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gdnkfgcun.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/ggfjulhiv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gsqihtrlu.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gxdueedbi.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gxsaxjpuz.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gjliyjndj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/geewzinrl.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gvcwsidom.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gpisdxufe.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gzbyosafr.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gflgbheta.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gsfsexutx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gowflzswl.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gripzuirj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gpdlspmci.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/giyfsmugk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gjklkecbs.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gylhrspqa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gtxftjhpd.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gjnooufsa.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gtmlofzot.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gloxtmdkl.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gxqqdpcfd.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gujnzfrnm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gapbzvsws.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gdhyrfltf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gfochppzv.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gmmalcsjj.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gigusijku.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gmuldtgpz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gehrxdibh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/geaevtxjy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gtaeayyer.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gneohyjic.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gtrbznsmj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gkulmmfyo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gzcgtciot.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gfxfipemx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gyvizthbk.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gdllbzmvj.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gcpewnzyp.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gubinuoal.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gmzuynitt.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gssjhewsu.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gsbsmnrec.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gpipfnsis.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gufzljxrz.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gsiiwnczv.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gswvqfsdo.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gpwwklilv.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/grgqyfjso.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/goltvwmvz.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gpzxeusjl.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gstgigjzf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gcwahwvbq.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gykgjakun.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gjoycrcpo.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gfifvvcgr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gvohdacfk.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gbsnlwnyf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gznhcthcu.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gnmzfjzyb.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gkrhdfrnb.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gjnybjigz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gywgnwnxe.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gnjzcveli.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gfaoqqvyc.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gryzmvaen.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gsmkbwfze.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/geriwvudz.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gstwkwxqp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gfbaowdiv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gsyeokvrd.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gdoeiajvs.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/geudpeoxd.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/giaefpotu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gnkwpkyqb.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gznrfbxvk.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gtxnnjleu.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gwvhlbkgm.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gkxzfdozh.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gjpkmcbgu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gzrnbxzmd.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gvpfcirnz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gfhnadlax.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gzkiuqjcl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/ggvnpjncp.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gldipxlqx.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gxdvuwdkm.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gsojvklgc.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gfcwjcfth.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gfnaciitx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gwibsdixp.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gjdmyzrkf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gycevublq.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gazecsphn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/grjlhmche.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/giicgfobk.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gihcaskje.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gbnzkpdbs.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gibohkjfc.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gdlzrekqq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gaxdokszz.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gdnenohpk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/geeaxqfob.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/getwqtvnh.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gfkxmbnyf.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/glnoyodfx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/glcloqvvw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gjgbzqfkg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gxqyjtvdu.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/ghlsxbftp.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gpwyudyzf.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/ghxvrwyjw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/ggldxovzi.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gxrihzvrl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gffreqfdh.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gfhmqjgtm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gevzflfrs.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gikpxlcvf.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gckoktabz.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/glncyxfxf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gcyagovoc.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/grkupjcfy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gkvwpetbr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/ghfodozod.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gbjdmuhpk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyqriojkc.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gmxmyhdcw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpwlstmov.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gsufpjhmt.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/glzhpvqrz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gsrbfffmo.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gdhlyrmjg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/girgmkery.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gsmmbunar.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gawzbmhpf.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gyvbygncj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gakiuhdbg.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gbgzrjsya.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gynasvyrb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/guvljktek.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gaxxtkyzx.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gdqrjovmu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gjffhorbi.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gkafnacsn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gcblkluqo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/geeitttcr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gfwpajegu.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/guolwwkpj.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gwgttsqmf.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gcchgmiwn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gmqjoooph.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqfsiukz.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gnkbscvbt.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gnlpnanrz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gcwbsoeqd.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gxezigdwb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gcfrylvcw.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/ghhpyjhiu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/ghdierulu.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/giiglbqwu.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gmpbgdici.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gbrlglays.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gptnhmqys.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gmiehzxmx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gpymsynba.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gbwdhaycb.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gpftyddem.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gklsatych.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gpvsihbin.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gxqjoejad.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gzetsenex.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gvezqwbub.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/grrcgfxad.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gtkhazwol.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gdqqvooig.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gsbqglafa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gjxbaqkpb.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gllkxufrh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gkyirmuqk.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gmvhionyv.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gsngxelgq.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gwdzlwizc.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gwjnotzyb.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gmzbbjnio.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gmnsgxyrc.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gurrpljtp.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gsrogyujv.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gddgrnzgv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/grrjwsrgg.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gcgydajia.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gblsqmiwb.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gsftnwzku.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gweuszksl.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqaclqhqf.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gppfpfpek.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gpzzqwxxi.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfyzkgenq.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gkwhrnctz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/ggniqdltf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gummrbthv.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/goacgtupn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gniqwuxzd.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gsvlyrzkq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gkaiztzxl.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gvrieyjla.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gspolgarv.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gdlwjnxob.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gflnuffez.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gnrhewilr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/ggihuokcj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gtayjsndw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gmwwtymvm.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/godmlldvk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/grouhuarm.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gkkchuoiy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gbgxkijjj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gpimvlrvb.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/guuddxmed.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gbbedvgyy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/grlzauknp.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gclbnjken.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gthbuinys.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gazeukqth.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gzdskqnak.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gqxgsvhsr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/ghyidioat.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gnnffkyka.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gljmkvapy.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gdmvdzqjq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gxjnivqgi.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gobsbbdpg.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gouessead.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/glaxryjct.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gvrrvltwl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gcfelsedd.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gwtefrcsj.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gntjhplxr.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gsnvlaciw.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gxhdzdpdw.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gfrxetxdv.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/goraxbrbm.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gmfmeqgot.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gjxczfyjc.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gwydieqqd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/glogpbkwn.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gvceufiys.sHtML


<!-- 参考信息 -->