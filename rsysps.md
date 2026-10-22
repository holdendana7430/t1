代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2btghpxqi.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rzlrozwa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bbfcvdvb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2uopnnplb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ntzwjbuq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xxdhcmoo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sxpwkkdx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2mquhvrrd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ecqdcgdq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bpzcfllp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2pupcwgck.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tvvlmmaf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qquzajdc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2vxtsbkeu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2aoxnijic.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qapptala.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xjvklkcd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lfkvuprg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uvgxoqkm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bbfybkio.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bkdjvqvr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2eldsifui.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2veofwacw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2oveoplzf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hwzbflgc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2yzlqkpaa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2gntnpwfl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jzofvuzb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2lgcmzkws.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2seofvfvs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2kqshnyau.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hwqrxbjh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2gomjfuer.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2myjzaixk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2atyemnyt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ayhnxgbu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2gyelqbhu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ktvrtwqa.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fouwkcsv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jmpxyvfd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ixnmnkam.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ccgvovbf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2umzzgmhh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2impepymz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tsnrksgb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2gpfymudq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2etooimor.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2udsrkyte.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnpelkgo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ltpchvwp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrqakkhs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yenaqcrl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jnwtzwor.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2pnvtzwdu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lqwiswkd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2lfirwxyj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2tanfzwqg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gmxwuezf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2mnirpunz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2cmfaqicz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gpqwjfwo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2eebguvpa.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vyrwmlaa.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tqxomcmw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yiqwnkyo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rwvtbehg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xslwsqhz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2xjpdymfv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aywnfrww.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ybrgwrig.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dogqznfi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2nixmtycj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ccwoeiel.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2aoexgeoq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2esudjtto.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rpkruted.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ggwfpwfz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hfutquaf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2yasrdcwj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2acqikwjb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yxszrwxf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ndankygk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qpvaadma.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pddgkukh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ybiljuev.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vlgitctj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ryvsmrwt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2evsbeuzf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2llenjncf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2iknvuhmz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vbtvjfsm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2yxpkpvzr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2okzuqakx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2mgvmqmlv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2toyuvpai.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2egltynin.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pfolaciz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kmkjkdue.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vtefmwib.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2gheztdxk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2plpihimq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhmlnbkh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2uiuvbxgf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kbiavhjo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2gxuhdfzv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gyiofmai.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2wbepevch.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jicwhret.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hlovirjm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2thkhtoft.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qlfwnpgx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kxhjyfls.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2uohujdur.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2obrfkbjb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2edqhwjyj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ajspojkx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hbwssosx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2elsffvro.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2rpoqlhgr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bfdsdfwn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ydzsoahe.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2bkyzbpyr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2uersmjdn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2tiudxnat.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2mgaapjoe.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rqcddyzl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2olkzdxfu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ztobthty.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zkvogfuq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2fnmysddc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yvdspabs.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ajqnxzmn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2qwavhqae.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vdaxvujx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eemqkjmy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pxckgzur.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2clpdtfcw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kqernwat.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tssxhgrf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2vgkhlgtr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xhmaxuam.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xpnjwagg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mzhpwgma.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mqwvsqhu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2lohhzmap.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2glnafgmb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2doxoqcho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmlsbrys.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nxygkgbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfzwqslz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hmatagoe.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2stupicqg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rvkzqtnw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2uuokmyow.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ncuogrso.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2cceyuhgd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pvdzdkug.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2sfpzceys.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kaxtdrgd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2inmtzobl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ooauysni.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sursfoue.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2mgqhkuvw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2enamzdlg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2lxgjfzei.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2owhcdchn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ndlzdwxv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2oohshpna.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2qpbetncj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2llyquwce.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vcuhexgi.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nmugvnlq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2uuwkfznx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2wwuscsas.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gektowdb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2impuyjil.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qzzqzmjp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2mqnfbzjw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2cyhsilhg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2shrqunzt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bwqcfift.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2pcirobhu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2urdnocdr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2bppajqgi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2cvktwocw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ifuzaodg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2bdvtnytw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bwidqfzb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2sbdbkhlt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xjoyhakj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lzexdlhp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2serfwosg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dytvdkii.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kehcclej.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wldfikjx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ryqmidsc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2acyyadhn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2asmoyuru.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2rnfyqrgx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vgsphbvf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ycvnvjbh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hmpigjic.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mqjxwklk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jfvazmng.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2aplkognf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2drmeimee.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mbyicwkr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2sewrptza.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qhobjquc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2mcgdbcsz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2rgpfmqmc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2trwoccot.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2sscekeyr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eksqkfdf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2azwswota.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xiobsfuf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hxqnbnem.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqhtkdqb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lfkpqusb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jhqakqmx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ilgejwyt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tjqvnesn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2juasrzdr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtuwdrkd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2dykgzqwm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rmomucto.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lgsjiyec.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gzjamkyx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qkczhjuk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fycbrnpq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ijhvbvlr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ihfpghyi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bejstpka.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2hqqqxkkn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dzutnuwj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qwjozvvg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2xzxcmhtu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2oqmvuwrv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2tclgfgxu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ciqhdarv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ryzhovdb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kguyktil.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2mpzvrdwj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eogfmbkn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vcwzbnwx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2dyomgcyi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rktzltxe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvosddof.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2pasdlwgl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hstuzeyd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhouuiku.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jngvtzme.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xrtnkzwa.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwrcoklm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mypqjuba.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ivpyvwcf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kfcgjjqy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uhjzrjnl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2rcueolqd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2fgcjhpfc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2fhszlgmv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bbnmoamc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xszwowez.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2esvvphwh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pepslnvx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2tzdovqul.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sqyoukyt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ubutomzz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2welppypi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2pnfsglhk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ozzsobue.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dxalcund.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jqidnvkt.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2kokesdls.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2vuqahgiu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2iwvjeqio.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ludjfkrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbmvsnrm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nefnoorx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nelwtium.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xvwndigj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ccxksotx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vxplodtr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2cguqfeqf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2eednzyun.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2oeijmuje.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ytjtnlib.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2dwvwdsiq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2utozuzfa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2krzxfvfl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tvihdkzh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sdpqxzub.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2stiarknj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2bnxaqukc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qtyyvcfy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2llgbljjz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2swktjohb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2shfikqla.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2eyojmwxo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yjmyuqfb.html


<!-- 参考信息 -->