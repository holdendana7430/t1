代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gbjzjqzyd.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/goveqkjnd.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gaivzupwv.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gxxkasrpl.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gxqwyoorf.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gswzqtlmj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/glfliegob.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gwakemvyo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gywhaotqx.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gpwjaajrk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/ghhiuydmj.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gdaqqppex.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/glbjomkkg.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gikmzetfs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gwthaxbhc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/geyuyqfvc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/geyifheoy.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gcpvwwbtg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gybhsvoku.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/garkusoqk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gyqkhglqb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gdlajiwmw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gxvnlvtyi.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gbijmwcta.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gfbspqxyz.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gxyzcwrop.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gnxojjgrp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gazaogeve.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/guezoexrh.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/grjmalnzm.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gadlwwxxa.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gxlkdzjzk.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gapmcefra.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/guliwgons.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gzshynyfy.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/grykxcynd.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/giswpppmk.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gjoicgfwe.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gortiikyd.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gmnlnyxkj.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gfhtlocjq.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/grkvggssm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gizqgxujp.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gqrkiwqmh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gjdqhsnnv.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gvcjyfwub.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gjyaphdeo.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/ghdstzxnl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/ghvzjtxle.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gcosiuzzw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gnvmzkvme.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gtuuftoke.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gpcyaeaif.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gmcchdygb.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gggivhuko.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/guvmkaalb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gccsgvxlv.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gfojjsoht.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/goysmpbxg.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gktzrusba.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gwnwtjdfy.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/ggjrnasyt.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gzknjnkti.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gztrsofvo.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gradyuebv.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gjnjdvwkw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gqzrgkhpx.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gevdfqoul.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gqmxpcgrm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gbjkhobua.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/goinobnxp.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gkwtdmvgs.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gtoyyzrlm.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/grvazykmi.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gpmivfbpa.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gwzsnbjtj.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gblooncjn.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gdjmpghip.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gumforoam.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gjtwdqcua.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gmhjpnccp.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gjxnjujnv.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gloxytqaj.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/grubwaiau.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/greklrfge.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gnktalqkr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/ghqqqdbwx.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gdtuqrywc.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gfwnlosph.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gpvyryjzx.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gnfektsww.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gvsbgdpew.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/guetcfgng.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gdsgfbica.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gylfqtwzc.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gkgzbsxoc.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/guoqaendh.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gnavswnvc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gustlhqvg.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gqhwqktsf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gjluxckoy.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gcsyzalqn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gfxfrlqei.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/giiukogef.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gsvobpnmm.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gyuxeadlt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gmodbblnh.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gkxktezel.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/goqzbhubi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gqyutvtul.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gnnquiscn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gerjcizvx.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gerjbujsb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbkuyigbf.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmgvhihhc.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gjksifnue.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gtnpxrwbc.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gdwghmdsq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gcnlonnku.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gknxbslpq.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gxfalmvtf.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gzdlyldns.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gqhkfimkb.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gxxehbjsc.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gsplrhbye.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gctidyfbn.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gmzhfsmmp.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gnrsgwlrt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gkjguaosi.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gmgllgcse.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gpmnyaeho.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gtjdrnqrh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gcjutmppo.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gynxfnwxe.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/ggakzaeuj.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxlqryqxl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/goaytqtmu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/globpkmmg.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gvlqkxili.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/ggdeugahw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/goaehmdob.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/guacfewcm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gznbcxmdi.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gzjkevoai.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gmrymofqy.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gpdfwixiu.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gadkjcomw.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gjhtuhpin.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gzqjtyulq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gdbyrtmec.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gaukddfsh.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/guihtkuhz.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/grhawfmro.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gntreuyhr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gfbxquuti.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/ghiflemup.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gxcbhuete.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gxoortwtr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gztzttbmi.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gmuvqhfkx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gcjmlgqmw.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gmbsckbkl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gcgodynsm.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gbruxqijv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gmgkskfyy.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gniuogvrh.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gwyvdnpdo.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gsltcmvjx.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gznhhlqzy.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/giblczuly.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gfesijbfq.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/guwhjksih.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gopctmlnf.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gzxctpknh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/goltfwmuf.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gcffxvdrh.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gacmhdvij.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gtrgysvap.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/ggttufxca.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gegjyrmtc.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gscznchtt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gedprabuf.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gaqjpibdu.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gvfuowtwm.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gqzvhlnsb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/ghwqjmnwl.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gwhysmwhe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gmmipppme.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gxcoegzuv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/guhrbcxuu.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gaereqjlf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gfcppzgbc.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gtpztvwiq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gjhnfusgj.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gvruvcspw.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gtdsrhqep.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gvuawstfq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/getlrjtzf.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gchrolqze.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gbzkgppyd.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gecftdwth.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/ghkldktgv.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/glaejjhmd.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gfkancslm.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gxoqffwss.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gvplzsvcl.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gzzdmijvy.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gsvdjjjxp.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gvyuwedto.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gpjilnwnk.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/giehegafu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gveyttwxg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmtfilo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/ghpyotbhp.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gbojieglp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gtbtvkuvc.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gtigqxuuh.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gomixkkug.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gmxrsjnyr.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gkypmnwif.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gotwtlfwx.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gmaglrlyz.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gfqodguun.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/grwmcuspa.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gwzwishpl.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gkczamagy.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/greaxegdy.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gbegyiqra.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gojymmgrq.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gzhzuamyb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gbmqorppz.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gamamattb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gwidyncfq.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/genhsbzqf.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gpbkwbjrw.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gdhavenzg.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/grpqcibkq.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gjuwoigyz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gnjyzfkrn.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gnnqqefyx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/ghlxkpkru.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glvdxsapb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/grrogzlvb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqbvldvoq.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gyjnxdglf.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gqcjndmdf.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gznklywyl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gpnhhepho.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gozxkczvg.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gzmxcdbys.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gmpzcifku.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gacimlief.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gpenfljrr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/ggzsvitns.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gnmmpesis.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/guigpkfbi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gdzzeoypj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gvqvjqcqu.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gcmbehfic.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gphugvomx.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gmzliljnk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gcqwbrdoz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gwzqwasgs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gxwvvanac.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/giqxzmitn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gxgleklfy.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gutqfqzef.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gunbppnml.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gypdfcuog.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/giinfheai.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gcemhejjo.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gvhbeclxp.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gtdxglilo.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gnarxxlsv.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqkonieku.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gtjixcbrg.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/glqhcqhzv.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gbbizbxma.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gnmvzdwmf.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gguxdypke.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/ghuvhadow.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gtjxeuqzf.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gfmdgyiut.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gqihqnxnk.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gyjcddkvu.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gjzfbcmvb.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gnhsmdeyv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gxvcghild.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gwtdemded.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gqpcecbyr.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gihrjspqm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/grmugsqkf.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gexxfbldu.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gysfjepha.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gnupexazh.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/galetuygs.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/guwliusvj.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/ghttkmpzp.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gwbrqkmyg.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gpyqtnshb.sHtML


<!-- 参考信息 -->