代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tzwwkshn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fqualxsi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2cipkbquj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bkcfxfhf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mrogcywx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2uhlpzkhv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tjsawvtu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vpmvdjac.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2dqtdctuv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tfyodsjb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2frzqapec.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xbasfxsi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2umxoyglr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2almbzfvc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2cmxrdbdg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2wmslwckd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2pljgriyy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2oebasghs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2cpvjpqvq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2qnyywpfp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bydttfke.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fghaihew.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2yokcrnjj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hemlvhmf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2txftmapr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lljfmeri.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2pvbxgjne.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2alhjpwct.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhrejfqg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ydfqkxdn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nxjdfuaj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vqreefvh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ihbkfddn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jragcnsm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vokkqnrr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nneczusl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nvbaackk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2lzhucnkl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2lzrsksox.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2rgnbjmnh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2psfkmlhs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vjeagata.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2gqvxjmoe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2oettedqh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tsrbeelx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2cmbabccj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2bkdzdnoc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2wnvnzurx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2sjvdkgtv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2pooupypj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bhxcjzqh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2wnnllvrg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xuxcewzl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2urcvcykb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2retqrang.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2dskozltw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2dktsemcm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2yhidtkyv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ldqsulhp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2teaugzat.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gtyouupr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bsbcltpt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2haagybgf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xhcwlfto.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2wgdnqjnf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2lcbpbplj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fnmoymge.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2lzdelkns.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ifxtcxiq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2meaneryp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hvtpuljn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2urmoegll.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2skmyycfy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2asblsffk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sqltndux.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mlchfayq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2bdxwcihf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ouosront.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2dfwmbugy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2pedjerxi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2mgofrfra.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2iyqolgus.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2oezbncbb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qtffxspk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2wljaewgd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mwqbelos.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rktuhhgy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2exdyvpct.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gsbtnbig.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ccphoeqx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rbrakcux.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2znjlvrrc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2gkihrfnr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ndrbegqz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ctdujkae.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ngnzplez.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2mqdyhkoq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2aqfsgieb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2flrcysgp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2yevvmfpm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2bakeinez.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gbblihmo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2egaqnzqx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2zebjkiof.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2amtrsnar.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wjitulpb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2gjljmeug.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ksazuhde.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2rxvmsvqo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2drsklgvk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2quarlzrz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2lejzadod.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jfiqskup.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2eoymjxeu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xqyaaxdy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kmvkbpyx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2alddaaoy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2deasfdng.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bnqkzhzi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qtqetzhi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2pixecbot.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ynxzzkcx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ulzvlvpi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2wrlwvjdx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2kdgcnigy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bjwtpyvb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zlpycmlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogheavyt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2tcksayry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnuhdezm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uoyxrdmk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2twwqizee.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ozcgohdb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2nuhxdgpb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2oxqbevel.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nlvfcckm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qybbbked.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jrdlmykv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ntmtucca.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dgymlvff.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jckipvza.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gpjgscss.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2aoiwjaiv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2azkvxqfo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gicpwufa.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2mobtepxo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gkeysoie.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rchagzbw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jxwzqjsq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ftfjzsoj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vgczqlga.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jdvrrhpx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wecisdyb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gqnytrhr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2imhyfjsv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xmmanava.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2urdtaemr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kyptmcgl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2davhpdeq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lxmqbsxb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2imbfjsvy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hhsfzzuj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2febvqjpm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2voxdpzqi.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cjucxhws.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fqkwretm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2odrrnugb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2crufbqnd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2moczmauu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pnhfwfvb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xwkqezsd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2gcuzwvkk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dbhfzdam.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2tmqdmybw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gsvtpemx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2alnachht.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ujnizdyd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fdjgynay.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ztotovrx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2zevwflho.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2liajwggg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cwsxadkd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2zlziqwop.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xjaxlhzd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2mvzcbevj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qcoptbrc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lcsqayxh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ibezrfww.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wubzawcp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ioqhhdil.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ocrpgevt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wrekmluw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2gnrvymml.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2roeavgbj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2livismre.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cucounqy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2etcsrien.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pecnrpob.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vysgpnig.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hbfpsafa.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pcpvevxg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pqwttnwv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2olfllswn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2dxqvrtcc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2sdamktjy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rgffkwpb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2mzivulvs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rebcxzfw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ivlhehik.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2urrfdlan.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2bdvnjwed.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hvlixeql.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2izsodrkl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2butzlgff.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2oizhrdeo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2vyhqbppl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wtyxxzth.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kcksvlrm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2msfoqggv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lkhujbse.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dolmqcaf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2atesxxsd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2eiosobto.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hldafixt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2axastsyq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ifsyjpiv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dituxsoz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbyizewi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lozzcqwc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2wovomlkx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhwhaedo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2cckpngke.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hazopcdh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2stsgybjh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vjvruhpg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2soqkrgrk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2akvfnasz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gjpnieph.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wftojivv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2phchokfc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xngxabsb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ksxvvdbg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2bjdddlqe.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2wgknvtnx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hpxmluit.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dghlkghb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bmbkepgi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2omcssyuo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilbnxaid.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ordedrxi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pwqpsdlf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qpccglxx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gqwuwyrd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2kaucegbi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2itofwsms.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nsdggsue.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2iicdpjjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtqbynpk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kqnucrzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrcdujbd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iwrogwqf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gdvnhcgy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gzhlkvqo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mrtzsoiz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2rvxuehhj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2himheejp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2sqrdanll.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hwlwrhxs.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lgnibqhu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2iztyxkfp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uyikflrl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fepsvenk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wjvbetfw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2saxiwkvg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2kaxklfwg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vsqkqjyz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gmnouhiw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2rmbhzzfb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2evrserax.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2seculffs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2hghubzkv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2vslhsjor.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2yswvymjw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qxzpzjxb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2oitpahda.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2uhyszlda.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2akvadtgc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2izjwozfg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ilucwmje.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2onmqbdzk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oijaieai.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zymythth.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2awvwsqkj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2cpsonahe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rtlsxcqi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2apbhkvll.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2sjgbrery.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ihmekiux.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jiwtpetu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2reozjavh.html


<!-- 参考信息 -->