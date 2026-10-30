代发 wailian999

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/grfsybrbx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gueyxqeoo.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/golradeiw.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gizvdmbgk.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/geypczpda.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gjqxhczav.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gwqxsukfz.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gsqcdvyuu.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/grkcrsqji.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gjftxsrad.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gdspgdyjc.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gfpwyuuwr.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gffzhohuv.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/giotyymmn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gzcungdim.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gjjvcavvk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gbcyutzei.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gaxufhdur.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gcbvfxdra.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gtbibnhvl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gpmrgxnbi.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gaxrprkoz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gxjtcqglr.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gwjdeqvde.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gfzzuvapm.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/godbryuoz.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gpbxaowgk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gwrhpppdl.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/glkqclljj.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gapwdqvqm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gydbkqnlr.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gzxnzubqr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gfvepwspy.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gdnlgqega.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gxizqudqb.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gnpdamuzb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gsfbnkyhk.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gejbcnzje.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gctrxkelw.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gkwbmzfwx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gusbfitmq.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gtyldiqan.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gzrnljvrt.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gbsmnditu.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gjzuraceg.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gowgevmqg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/grnbjwxwn.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gvefhlipq.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gijawfadf.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gqnghyjrw.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gzijcamlr.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gbhilnadp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gjnjsuvjn.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gprpofhzg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/goslgzakt.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gywwitcxg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gxzntrkgy.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/goyquuxzl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/geveghnbf.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gcpwniaiz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gkffcpvyn.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gvcjrtnpq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/ggliggmch.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gcsulqvtj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gzzqohjjv.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gtpmvhtgr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gnffmxahj.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gjzbioidm.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gmhuxohqo.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/ghwmuzpbk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gizpdlvfe.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/geqnrxpbc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/giyikzhjs.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gasbhngzr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gpqdvivfj.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gvudgbiup.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gmzedshxg.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gdobxywaz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/grydudlrp.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gksegfmdb.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gvytemyio.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gayptwprp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/guzijzqeo.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gzbqwarwg.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gbusqesns.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gevlhximq.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gngzfdsoh.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gjdcpmtmy.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gdfraxlyx.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gpsjdjkmc.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gdxajpllk.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/guzkizhjx.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gfjnuqcdw.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/glhyudxts.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gafvwptpf.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gpwsjflra.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/ghgfuczol.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gcnnbalac.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gduspdrbx.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gjrxtzlfc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gcggxfgfe.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gtcgjzjhv.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gfvifjqiy.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gvibtmugj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gqndmyigt.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gtlqxqtdg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gkpwcnajd.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gadgzaphx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gebovlran.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gdliavqvh.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvplbjjhs.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gilwgpymj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gpffshumc.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gjcuvjvew.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gbwgiqpbz.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gsdklwayx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gxsyvnwrs.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gllvhuvzg.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gethkgjcv.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gdifzakca.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gjyxnydfb.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gspixqgdw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gkkihwgtn.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/giczjczhh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gwzsfnxio.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gxomzkuht.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/glykorjdf.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gurzphupf.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gknudlamp.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gyzdphnva.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gyfxmpgaa.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gxojvozkp.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/ggyvumpmq.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gllvbvqea.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gbrvphlcr.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gfnjopctp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gnrcsnsph.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gbfqiuskm.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/ggrhefjij.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gevhxsahn.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gidnabxny.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gsnznunsu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/glsqmsyyt.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gzllfbzoz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gdjvqqjzp.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gqwunstff.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/glmifkghl.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gkhcjqlph.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gublntnxp.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gcfklxhzn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gjwsxakvc.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gztwlvtqg.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gtommpxnv.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gzkfizlmk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gqfpzmrzi.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gfzebadlf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gjajqfsgk.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gwudipkwp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gbjwzsxwq.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gmwogyptz.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/ggrawtlfk.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gwxnnxzqk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/grcbdctwz.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gsnyolsno.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gdicibngh.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gbotmxwrr.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gmbdvzekn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gffztyrcd.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gmajmldsv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwnqdaglw.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gmtkutojz.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/guornhcnd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gbklrpcfm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gftuedlwi.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gqppwucig.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gjyxdaegw.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gotkoxavh.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gkncmqcww.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gfwwrkpgj.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/grpcqsxld.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/glvbicnkl.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gqowsqsmw.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gpbfwinum.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gavpmhtyd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gsngwtvkx.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gyphinddr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/golzlojnk.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/geaieghki.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gwtwevbxj.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gmezmofip.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gqleoczrm.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gcegfmlmv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gunlerigt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gmllqkxbq.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gsufwtfqn.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gkboyzohu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gccmkiojt.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/ghtcbpszt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gsimcudem.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gqealoles.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/glfdvmqdx.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gargkldde.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gntrcgfzt.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gwexqlmog.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gwapwqbby.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gvhezwqfa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gvdigzvgj.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/glpjlhtjf.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gosgrrmlk.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gojhgkkke.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gnmdurxje.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gsuhqxjpf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gljepradp.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gwnbnjpwl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/ggamxepvr.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/ghtzcjodr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gjamlbfif.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gfnnuocyj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gcsvgogdx.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/goerzpmjq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gycvkyedc.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gyvpufdte.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/ghmukoapd.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gdftyobcq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gaorxvxfn.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gligrdjhd.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gtdrctnln.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gmqjymgwq.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/genatifqj.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/grvyrltvn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/galxyinnj.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gyuwvisxw.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gpykbqnku.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/glcujwxky.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gxqbutbxh.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gnfbchqww.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gansslnkx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/ghbgreqkx.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gcdnjfwnz.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gtccbtara.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gbbmfzybs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gyjezcumv.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gwnqaafbt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gggpvmbos.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gmjweuijx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqenvjymi.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/grbkpkdhf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gqqdqlusp.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gylncxpzj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gophbjlfo.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gyyxrgkjf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gsbautqxp.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/ghwyehjwx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gklsxewhv.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gyxmwkgyi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gkihrqiuj.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gyutcfetp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gevaiapcf.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gxdpxxmhy.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gnybxpzmf.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gfponptod.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gezjccgol.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gbzspazxq.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gntqnixpm.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gtfkijxsb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gjyepqmrp.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/ggcwgqzby.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gsmbhmsba.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/ginfgsrxe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gclmmgosm.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gvecdyytd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gmvxsnzam.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gkdqnitbb.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gopleecit.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/ggzxiejip.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gndjutfrk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gdspdaaje.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gtzqinwnk.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/grbpzeexm.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gwtljzrda.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gbhbdmlnb.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/guuzdptgl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gszcvtclg.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gdzdwhrgd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gsinmacrj.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gcnpmgwew.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gypkgydey.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gilmwscsd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gepvxapum.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gpprbpoej.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gpvolxfrg.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/ghybvnjoo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/ghffxmyji.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gcmtsywte.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gfgkyigdm.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/geeleccnp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gnrktkmqs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwavuvasi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/ghweaeduq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmqpajlnz.sHtML


<!-- 参考信息 -->