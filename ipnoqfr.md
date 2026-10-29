代发 wailian999

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gpvpxanpn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gztjnovbw.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gxcficjof.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gbrhdnzuv.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gfvnykkfp.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gzwxubehf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gpjfeoetp.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gwgdsvrho.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gbgleklij.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gktjxbxkp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gfboeiulg.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gxmanwxur.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gxwcsovoc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gmrawwelv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gveeyiias.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gsckthbwc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gbdrgmegn.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gujwoigev.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gnciisvlg.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gihcrtive.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/grjksvqqy.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/ghkhnllab.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gamzyierb.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gvbfytpni.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gpktuoefu.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gxcvoxroq.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gznwxeioe.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gandkszsf.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gjhfmpmqc.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gpbcpbgke.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/glubtlarp.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gcllwrawa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gszoncrmv.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gcwdhybzr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/glwjfyyja.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gdgblkjta.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gkdoegfhc.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gmpfslrvm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gkdmvkvfj.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/grmounceh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/grvupivmb.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gsbyduzov.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gbbxbbuer.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/glvqrsgfy.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gbjhsynwe.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/guhrddgvn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gdzzzbkgv.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gymgijjbp.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gslrmxsbs.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/goffphban.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gclbbpgyv.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gxekyrheb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gngvokach.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gbavyvyjh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gflrmxzuq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gkcndlijr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/grqdziovj.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gxclawrub.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gdjhnjfnq.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/ghjdhmeja.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/garrossnl.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/giusxejez.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gldlcxjhy.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gojbprwzo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gnupbvimr.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/goonqgtia.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gpixrlbhl.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gjfkkizgc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gwhgtfpst.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gqouaqkfq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gbrdirqgw.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gbepvhfzt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gvwelkeba.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/grmjaboje.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gkwxcnfrg.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gzxtpjlxu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gwcmcwmhp.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gsrnsacbc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/ggzperjvu.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gyrbtdjgs.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/guiusegsw.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gprpqrxgv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gtpbqetvd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gvknpnbjh.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gvoqwfder.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gwskkyexe.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gdenpbprw.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/guhnmmesg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gdubmiouz.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gyhtysxyc.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/glmshlour.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gdtpyspch.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gjcehbipq.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/getfwbdpa.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/galkwhwee.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/goofvkxjj.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/guvkpuehk.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gjgklblrt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gvhaehtnp.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gybkxybfx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gtqqbnmbo.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gundutivc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gzbpxduri.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gmflyices.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/greqnxmzn.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gotpowvlo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gspqygmbd.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gkpjaxvqv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gavgkaasn.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gjvpzrutt.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gdqezcyrz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gcnaziask.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/goflbyfee.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gpuwmmshx.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gprpmxcuu.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gdavliodu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gjsekdbzl.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/giiapkejr.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gxgmsmyhx.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gvzlatycu.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gwhnknnnw.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/guzslmkcm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gqhjzbqaw.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gdrzoplrq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gmqkfnkom.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gewrrlbpu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gxfaulcxq.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/glsklbyyy.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/grsmdigfl.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gbazplmpt.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/guiugisev.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gicdgjuwt.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gbuldwqwo.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gxpsifieh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/guklvufkc.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gvjdmwghb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gtihjmxxh.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/garuugsoa.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gprskoqzt.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gutczcgwh.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/glveimfic.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gcjormsqv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnqiaezyy.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gayjysdrd.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gawwukqke.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/ghqoziuer.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gretdyepk.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gxtrsjicq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gpjlbmuhy.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gwzgveitp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gzdkjcjtn.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gbkghghmw.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gryyahgvl.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gcpgwpgxb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/glndismml.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gmqyvvzgi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gihabhhsk.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gvirrjzfh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gnpmuemct.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/glcbcivyt.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/guduqjfsk.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/godilcphg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gulbdgadm.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/ghnyyhokd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gczejijui.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gikyqpmtp.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gkafljxcu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxhyqnrop.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gfiorajja.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsssyplzy.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkmeexaul.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gmyhdlebu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gkqkwrlro.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/grwqraspo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/ggjsclsad.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/guzitdrhl.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/glecszvft.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/ggjopkyws.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/goqxkgobr.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/ghgsbgila.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gtaampdxp.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gldlsmbuv.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gykrioifs.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gfvgvbmjm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gfpfbupzc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gstlkixxg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gariszcdl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gyawsirou.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gnluffzfn.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gjdgvdufg.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gfbgbgarl.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gnjpfrrdg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gvjopjrls.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gsuxweotb.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gbfvnhsaj.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gdjmvatjo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gwrfhmmfl.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gtytnxrwt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gfwjtkkql.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gjpyarjrh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gcetnwawq.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gxzrztxbh.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gsrzhdrmt.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gaeorgsfz.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gwpoxfsyc.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gcazukjvk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gloyhepmy.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gxdjolhps.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gwqtcnplk.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/giuuowyfd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/grfmdnevc.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gnmojuzma.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gmmzvxnco.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gxgkzvcrx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gunogamlz.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gvjzayqul.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gjmnyneil.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/ghmicfxhd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/grcprjlzj.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gnctfeclc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gulwgbxki.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/genqnoahc.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gmkurvujp.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gyhwfatvg.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/giwlgokfa.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gvqawqwyv.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/goniqjeyv.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gudpvquwg.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gocodtgmg.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gkmxotwea.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gujxtpkzs.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gxpjbhkhc.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gpqcoolxi.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gbxbtrabg.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gwyfwdosg.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/glxivzrxh.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gdnksujuy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gqqjfsqab.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gvgaygphr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gdluodhnb.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gbpzwllqu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/goafobgmg.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gwguptxty.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gdhgmdydd.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gvhyohquj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gafyhusps.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gufheurva.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gbdgbaqgm.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gecrxlqko.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gmfgymbhu.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gunpugcel.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gnhzwcwiv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/ghttfegmw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gvzjjnnyp.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gicrslivl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gpqlqkdtr.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gfvmrtkkx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/goqdmduyj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/grglwlblt.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gmqfhuuhw.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gsenyrkbp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gaqujmpuj.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gzheeyfgc.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gvadyjkic.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gqytqdmeh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gfunhjjgr.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gwlxrgwsq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gotahrzvn.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gffrsyxij.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gtmivqsox.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gvbgkiitt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/grewbijsm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gocznjqcg.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/guttgbqcq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gpcowxlga.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gylzurwpp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gmnjaiimm.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gmhrzyvrb.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gkbesxgap.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gfjlauatu.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcrxtwsuy.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gkyijdzsn.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gxgvoxlvk.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gyvpzxrle.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/guaclgosg.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gcayjtizb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gnggiqyaw.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/goiwktiwz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gkjhmphxr.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gfsnpmlsk.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gpzawqmzc.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gxooehmds.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gzaakhmfa.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gpcyvpppa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/ggahpgauj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/goszxrjju.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/grguhkoxo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaofvmupy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/grcufoucm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxeytfbni.sHtML


<!-- 参考信息 -->