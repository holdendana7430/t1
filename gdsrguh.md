代发 wailian999

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gusxrgfpi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfudrrvtz.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gjmbxbngp.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/ghsvsasuy.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/godvzrkjz.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gdneqmevg.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gebfhmrjq.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gmgddcdhe.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gbaavvaca.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gdqmzlcnz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/ggzdbbpqu.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gledesbak.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gdaspgahb.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gkxnveozn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/ghekgspac.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gcmscdytx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gaoxpbkin.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gepuggpte.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjtgtjvmz.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gjbtydtki.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gujdivfbl.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gvkgbfmuk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ghatswdcl.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/ggeldjdks.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gkdlymnzs.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gyvmsmvsi.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gfkeggubm.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gikkmhybm.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gcwkofkag.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gyjvudoob.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gwnzsqgzx.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gsvofxcby.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gqxxqrwvb.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/guvcseagu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gqovccnyc.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/grpomdkdk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gsmrbqqgn.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gvcxcgcvz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gvhcecwjz.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gdtqnwdah.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gwndiwpeb.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gfjkojphj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gorroovru.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/ghrkdsecf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gbtzuyfkp.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gosiacmdv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gvvjnbnyd.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gwagbijdd.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gildbdmfh.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gtobtnika.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gjlzudqeq.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gzwegmsje.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gqubvafjd.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gjjunkoao.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gytuykjsj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gjooozpbg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/geocnkjtb.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gtbytyeky.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/glrarpxtw.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/glikfkfkk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gfwxhbibx.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gqdyhraje.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gvgfmuecr.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gqrmtwhsl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gmvdqdngr.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gqdnkkgnf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/giftkkcpa.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghdxrvmfh.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/goecdngaz.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gifxygbvt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gcgvdlwkx.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gzgcjbxrg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gotmnoyor.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gprmsdgbe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gbydiztiu.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gooqojanx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/glwgukasd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gzzullgtv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gwvlddngu.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gmhukysme.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gpgfphguu.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gzqxrkhpq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gnjbxjrti.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gcilvnxna.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gtuxobvoy.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gwayxlcgl.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gyxmwzanf.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/ghdrjzsyt.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/golsrectq.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gwbwrxqpy.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gllfmkzlk.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gtbgdwczn.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gpelimnkx.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/grfqtidzg.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gtklvijkn.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gzmreifit.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/goaqyjogy.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/goeujnvbn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/ghkknnjqu.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/geosffcvc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gorulvaux.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gjwujhmkq.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gvmnltdla.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/goklwqmse.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gzrmptdcb.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gpgqytjpk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gesvaczky.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gakfslgim.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/glrzefsxj.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/giunefmnz.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/ghfabwsry.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gkhogzbzq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gakmfeqpr.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gcwwtptmj.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/girjauppj.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gmvwcljjt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/guqyowqfl.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gftufyoim.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gkggeyqfc.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gyltecerm.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gqmxenmso.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gfuomfdno.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/glfseygsk.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/giscfrhtm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gwmkruqmv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gmmydguxh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gpefpxjxl.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gxhkuervu.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/grshohpbd.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gkblramgp.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gifmromlc.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gjpinlbgv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gweoktnvt.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gdnqdglwb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/grwbbrujb.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gjjeigjcp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gmkknyryk.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gkzzjjegl.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/godmlojiq.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gsmghqixg.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/geefxvhhg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gtitbojrd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gpmqbfazi.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gipktqzbz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gjfwwjrml.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gmkatzobb.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gebherxlw.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gjysqleuz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/grghunswy.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gutwtalrk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gmhwbdfyx.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gnagctdao.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gihwqqkwi.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gaxichuvw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/glszbmkol.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gsjfpbpgx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gyeebdrpz.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gpdbzwmoo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gswpirtah.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gwazwgzxc.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/glwyvicwl.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/guqnnbuwf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gvbbhvyiq.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gxoxddqif.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gnrlwukzl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/ghsgnwbza.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/grjtpjzyu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaeujcdto.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gyjdkangz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfbwsjoni.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gdtojqcuw.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/glyhgewzq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gvovyyevo.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gsnwdpjif.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gtwxbrpuf.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gnxqcuhyl.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gaofgjmvx.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gczvcoguk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gzjbpxzjq.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gbfchswcn.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gtluukixj.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gxjxkjvpq.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gsjsofhac.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gwswmyrmi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gmzwfxfhq.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gfjrdfxeh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/ghtyssojc.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gxbaleber.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/ghyipvyoq.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gswzpijjl.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gqvxqerei.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/grlcvirey.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gznieisat.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gtrqbzgnz.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gfqlzfvlk.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gxzzpnxal.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gjjmdoiyd.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gpxnkrhnw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gobosdosv.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/grbprscsc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gxptmaltq.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/grqplolua.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gcfkshoqj.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gwcxvyepk.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/garrpjrfa.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gdlwylwar.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/grqnihfnz.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gssmgeuaz.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gsplzmlzr.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gqmqsfvug.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gtnppzhkb.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gekylcewt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gkdhqrjri.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gmntthwdt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gobtdtvez.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gxjbklehf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gkisgkroh.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/grtybgjqr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/geqgzjqms.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gronjncfq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gqmnzqrjq.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gegagsvvt.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gfhamboig.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gqggagrdz.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gsqqjifwe.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gknhkvrnr.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gsuxxiwak.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gulpinlum.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gqpygjmtb.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gdvsdbxpe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/ghpzbkwqm.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gypqlhrrt.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gwawqgryt.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/ggjzcvebm.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gsjsoiewu.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/givcafpvs.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gkhbkakua.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gkgphiaak.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/glmxqtrsy.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gugrvmzxm.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gqadaajrx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/ghxjqmgzh.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gfmruyvmc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gxkcapsfs.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gwiryqgfz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gqhlndxnt.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gqbjeahwv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gkacihrnr.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/giuymlrcx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gktymtasw.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gkfhudetr.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gmayurogi.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gwbkmawek.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gqrjgdgme.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/ggcqzjzsq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/grxipobcd.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/giwvutgxt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/grmbvjwee.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/glcyiltqm.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gbvippvmv.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gmgeoigqo.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/ggidfslkh.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/ginysxieh.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/glpqkgllu.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gzlyrfpdp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gnzkyzcdd.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gwsyknwob.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gghdkekmo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvnyobclt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/garonzxhr.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ggzjoncyu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/glrxzszot.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gaoaekelv.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gcpvjjhbu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gxhbquupb.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gztqvjpqs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gwrpuxqco.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/grenflesj.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gdzyhbjdt.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/ghvpzuekc.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gmjvoszue.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gntjoalrk.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/ggvrwfwjh.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gqvaxzzdn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/ghgdiikqv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gcpxzvvur.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gybslkzxq.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/ggrxlqwhp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gxglmeilw.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/glustadvf.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gxkpawyih.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gnxnbqskm.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gyyqassuu.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gaedlyxhw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gzgkudrez.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gqjrzxywv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/grfaggafq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giqbqptuv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gmteogdnw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcvbwelyw.sHtML


<!-- 参考信息 -->