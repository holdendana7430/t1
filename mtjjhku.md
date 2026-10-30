代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgrqcgoq.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gbonbzski.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxendhdgv.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndqduzuw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgovzbfr.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqoronio.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsgkrmlf.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrosythy.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwyrlhiyq.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbxbdzdd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmtdikdsg.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcpjkhuc.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gobrqzeaf.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyyysmko.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggghiiufp.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/grptlnzzh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gygfhlfxe.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gutmrnhwp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmvwpmcw.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gyjixperi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggybpoxev.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaxfdfuz.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgerfuqz.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziurkxqn.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/guoxypsme.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gegmvmooo.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/garqeteoq.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gycefdfhg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/giqmmtiof.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gkimwlnsy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gaxhhhdye.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlnvgnpq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzjguzvwj.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gejdduahx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gujovprsf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gammnyfqu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiihkego.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gldgikgba.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyozxuatk.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gsszfrnic.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbytkjcad.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gsmvpzeoj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdewjblgc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpiiecjr.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagnkpwgl.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnreutipy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/glkvzrtdp.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gqupytuti.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/glweoajuc.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/glykbnxds.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoiisect.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcrdocpk.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gwenrsusc.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcpbttjm.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuhpjxuv.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gslvnhvzy.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gizmtxhbt.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gotufipqf.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gczwoyrds.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvhxzmfr.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtksbcseg.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczpdbjvj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlfwnzel.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdxooxmtq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gutcxknwe.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/geuqarhno.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfzevwteh.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwelkzqzl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/genmsnmha.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gvmzaaopr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemhvymiw.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gcluubmmg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gempkuxcn.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/ganushohv.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqgcribxa.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gghpjjicr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatucvgai.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggbbrowuu.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpzwuftba.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gsserkvog.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gtnaywbnl.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbsrzxhl.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gcryshdik.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gsikowgvg.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gnpimpmvz.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpcnizht.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdhomghs.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsxxhhip.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmebhnhmp.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gzexkmadb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnzdsvuh.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/grxkxolhk.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gzkuorbqz.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiefrfvz.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgsmwoli.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gujrzjcgq.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/glueiegdu.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gydweobzg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gysklgjrs.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvtyaymh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/geqiaancg.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gjjslkczj.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ggspibwbn.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmytzwrvr.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewqrtzaa.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/grkunsxia.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxwckpni.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcfptdbv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdzyekex.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gjvxvkeka.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gjhnfxlle.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqaqkvoo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidzxvcti.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gunueixvk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gicvtbnhb.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmrasgnx.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvjwxbvh.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamyknmpl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjplnvuwh.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/giojfcjgf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzspbaldr.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzbsmxrdn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gxrmmiwbm.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gjtlnedbp.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gycclsnlw.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gizyndvvn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxswiovax.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/giaevuuou.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gixgdxbtn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gturwyusb.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gfdmdtzuc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzcbdpcbj.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gksigfdyg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpsifnmbl.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvnzmrlzz.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gjuxyxgvm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqfcjkng.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gqvoujfnk.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjytguzcc.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtshjewyb.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gfarwishg.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgekqtkd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaxjngtk.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzhxrqff.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gggebkixx.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guunxiabw.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gxbddiftg.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/guqkswehe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gburnnoha.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/ghxtlpzdj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/girskqwsr.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gtkupozjp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjqoydrl.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/geqdivcjd.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyonatcup.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfpcgkrj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galfosehl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcnmhagc.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxgxjgcq.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkohvxfya.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gqrwicdcx.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gwupubfoi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxweqlcrt.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdvyzeub.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gasffpsak.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gzbaqvbpp.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gjvwkentz.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gjgqxmtkl.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkehjohcu.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghowdrawr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gapodbpps.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gibzegoly.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphyseqsd.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gytgkfhhi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gcqfbomya.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjzxagiu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfshjhjtl.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gaubhdmph.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gjuqlijkv.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gesbbwais.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gfxwdlmjz.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkgeqaub.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvqysukr.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxafnghp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gnjpzxieq.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxctucnl.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuxdxugb.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzixobxvw.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gascgksut.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqelbyqs.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gywwnvbip.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gofxsdmok.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycvmsvzr.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gusfcflgd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuvywfli.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gzhcfwmqu.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/grasnmvqi.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gynczqyjf.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdgykmiz.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpmcnmwr.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/giykyymcf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/glgpsypmn.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxvatjpnk.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/ghcibqeor.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gcufgrhnw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmmhmobd.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgdqflww.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggivhmiqg.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllxgzfaa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gycgrckmi.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlvcwsdz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdqtlizsh.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gheoobcuf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gqvesqwys.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grarqrvpg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmuidkqz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbhhztwq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gqzccxonj.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqlehbcw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gnpslnzng.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmelakfng.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjqakscl.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdtckwui.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/graeoplxd.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpkmzyob.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcafurrw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkrwnnaz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glpiltcni.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/ggowxhytv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gkotuqgww.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeidkkmw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhvjbaji.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gykwdnzra.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcebyexm.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngztukxs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewstmzlo.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxciappi.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsotckgzx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gwhzoqqnr.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gtkzeukfv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gbtwoguan.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gekqarknf.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/glwgzzgan.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvzqxryv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgbtvyqm.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gisrqgcgu.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggddmfdor.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gilkqaeiu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/guorffkih.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvxqjaaz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknnhkufz.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfmriibl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geulinlpm.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gsygcbtak.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkizczvns.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyqovlwa.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnekqsknp.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gebsdbthz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gquffvpnu.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/giqvymlcm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmrjilwy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqywabydf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gflwpphvy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelxhfhta.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gephyuoal.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ggijpgpcl.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhostrlk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmcusgir.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrlavuvm.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gkmcejbkm.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gwgzxcody.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwygjjcv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagzbaaxg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupleeiwj.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gzakjnitj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaxkjrso.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/ggvqjhdcb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwjwjfaas.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gsjlzgowx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgoccpvi.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeejknqb.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gpttuhlgr.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/giuuqrqbo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gnoqvsztl.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gohviakww.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gpwgcwjtn.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjtwrbeb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gmlgzwwca.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcxexksy.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gbibxxewf.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gmhxewqjl.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldrhkxsi.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/guxcwlzkm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gtqkciagy.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgpyhcym.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvujujkn.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/grucfwxjs.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gkknsdwmy.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkclbwgut.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiskubac.sHtML


<!-- 参考信息 -->