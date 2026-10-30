代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskdgvnsl.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gibakullc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnuubquy.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gebqtantm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gpszgjqdw.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gfbdcuuuj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gckzbrvcq.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbupcsvx.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzezwchu.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvedkqosw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhwjidnu.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gbklwyykq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ganbzmgph.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwapijaxb.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gmpmllawb.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gircfpcpj.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gjutpvszy.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gispahwjl.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvycadvlm.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhjrjqxz.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpcyfdya.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gnajqfktj.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gpmnktkzt.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwkzqshn.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamushpxl.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gcemyeijv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlhlaxqp.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gewippjcw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyolkpba.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gppvkxfta.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqverkkol.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzsvicha.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/googmxejl.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoaqhqbx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdmkneetm.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhwisofa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuifdlaa.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjklzanhd.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbmttbdkp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgkfhjde.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/goiqpzbar.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyjqhgxep.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gowyuhfqp.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gejsaclbw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/grwyxjnco.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyyctkvb.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwsidlln.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gjzjwpwzj.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkfbrwnr.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlqmcjfm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpvxphzo.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gspzqpcmu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzograoq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrjgnnqq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gseksccfw.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgnmqujl.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhsoyxqy.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gebyzcccc.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfwbhfov.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gwblqxnsk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgwfzmnq.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuvuhkkc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnunshdg.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkjvzrxt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gbwwpzksd.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgmwgoym.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gzljefntb.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/goobfzbqq.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gviapqzat.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gljhtdndu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjepwgbec.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/glnkwlvzc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkajdvef.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gwonafscr.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhfaakmj.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxrhtyme.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkbzjmgb.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gxnycluwg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gobjckamw.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfhtszon.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/guzprtnmj.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzxyqrua.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfqefafyg.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmmssyrk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gkfzajnzd.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvcedahca.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gwfzaftke.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gnxepcvpf.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/ghexkmnod.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfjyiahc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpvuxurx.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/geaypjiso.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gymalvfez.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gomnzddhn.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeporzxh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxabnewjy.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gjxxycbog.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxgtpraaq.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxhochxp.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjikwnnxv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfthphnyw.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gardzxcah.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gpfkxmfjr.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gqzcqtamj.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gceqcqfeu.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfstiyvnt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/ggeuipnzl.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/ggyhfbwli.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvvyoqjd.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gbzriyupl.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gsktubdpf.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnmglfdp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gubbwtbra.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gyvgljtos.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/groopovuj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gossaitod.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhbxsyyk.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgjuymnj.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/guwhskpsl.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtibvnxwv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gpcawlihw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboeomjia.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guptugdec.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyvnolan.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gguuyyelo.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpgsxxbq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gtdtiezts.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gsbjlmqpa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiimvzdr.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gboksyxem.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcvqwepr.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpptqzev.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnawvvlne.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gseqgfmta.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gzqpuijly.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbnecmhn.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfksodib.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcytkzaz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/glbcopirv.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/guaxawfme.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/guyjakjbj.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelmldexm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkshrbzif.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvecsibvl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpelszze.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiquczeg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gtzisjeis.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwfddfqf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gknmysygu.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkxbbirt.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gftzpzltp.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/giilvlbpm.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqqgsejm.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gnqfozyiu.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gezmbejum.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gosqzpvck.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gpfwkuitq.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmodzibd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqroxwsuv.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gomqbcoui.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gjgmbboix.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gswqmaiaq.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytqvsaql.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmhvjtubg.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgmpwyry.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdroklkji.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxcfcmol.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxneybil.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkozoxzjb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gwpulqyqk.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gscdpfvep.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypeduwtx.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuqxofvp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdytarwdh.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gqudwydjq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkvlwmrv.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gmdcifjew.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpumxbucp.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbyftbbc.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gcddolbhx.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gelvqopap.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkzffpip.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gmyaxlyvv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gzpmvsnaq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwgrphiq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gndtstlct.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuswmsqc.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gnbbgmxqs.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/giitijluv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvywrqrr.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvsstzxk.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyvmdsqly.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geatmcsmu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzwprxnf.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gegydlszv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwksxgohc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezelromv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcnejxtdw.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeufiwyu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gfkjpzxfy.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqrzfacg.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoohtfcp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxifqavp.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/glhafnltj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gwyrxebcb.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghioeeccf.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzgnymmz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gbaifolzh.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/guopipdnv.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/grhqlvied.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvqzhwup.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoqgclbr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmhtwryv.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gemuyzpcv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoejxbzv.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gvwpuzrdy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsqbnbmj.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwpyxdpq.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gnuksicgf.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gzffucndy.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoabkvpf.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskvmqzdh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gdmqjbzqt.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/giamjnuzo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuiqusrc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsogtdsba.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gywoohyvh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gaxjqxeyg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gbsgvpjrw.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gtincqryt.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqdcybic.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gtxjsqxtb.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/guuzpxziu.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gvlhdwdim.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkokrjrl.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvhkjvut.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gqauaaduf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxjeqzcy.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gifobumwy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqqrhuga.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/giayzypfs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkudtmzfe.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjdflfyj.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gxjgulbzv.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtableqlf.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gxybsvmwf.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvcufbfj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gboufnxap.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcaiodap.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdjurqgc.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvlocngx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbumdlrl.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gofgnhpec.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gflgnidpr.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwyqnvgh.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwivqypz.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gigajrjsa.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gfstsltnz.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grfwljshl.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhkojidg.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkihykzen.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvgepnbj.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphcdtdgc.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gauqamvqw.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gohuuynpv.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/guxfihsdy.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gpggjsqle.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/ghddkhriq.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gknfgblia.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggenauxjp.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gjbtfccbt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxmpqpxmo.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrwjfvnb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/glombwbbs.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlknblpb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbripkotl.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnhqinjg.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvanqfih.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowutojuo.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gvzahzosv.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqaexzpa.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtaihvei.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gemjmyrva.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaaffdkl.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gllqvynoq.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gycykmpgn.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgguqjzl.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkphfiaf.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/guvqpnyvv.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwroraeig.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/glwuugdtk.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbvwvtfv.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/ggzisfhcm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gqpqabchd.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyviroop.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gadylzovy.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gtftcyjrs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhsyuqat.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/glgmopmza.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gfplvfnuu.sHtML


<!-- 参考信息 -->