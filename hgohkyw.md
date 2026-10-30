代发 wailian999

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gnpviqnou.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/guvxpiqjf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxaditqf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gncuqopoy.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdbwcfvf.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyckdmsq.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gihbteyns.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxeclodo.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpcmimrf.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/glzmnaasj.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyzzuoai.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjomuzar.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkasfgjb.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfdyltsf.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gocfcqrzd.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gwoqrofim.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhupezod.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamfwvdxd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gmssfnnbc.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwjhnnna.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxnwifdbw.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/glceaosgm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjxnsmsb.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gumglukfz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqfblfew.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gohypubld.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfmfeizw.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/glsywyzdl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbsvmohj.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/grbcqgliv.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggesdwjpa.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gscglhetn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/glpuojmvk.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcikvxxhy.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqkkuarv.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbraryox.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gznqyazpt.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gvddeqayq.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gpsszabap.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqkhbrrl.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gnlkzlqzi.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhhfsrkw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gffblsygo.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gltmjyqgi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gxybsbuig.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwtyuwlw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gztexuycf.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyumamtj.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gfaatzjdv.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnuubresi.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gpwsqqicf.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gahqfufkz.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gmmplgvdp.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiijypqe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihseylgz.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/ggrqydcne.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhukaeev.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gfsjjlogy.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ggypdbfqj.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyueoebsx.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gxzoumrfm.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gopvcvfal.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grokymjrr.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gjgoqbcvc.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gjeitlpqt.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gvzdhdzjl.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gtdrvnual.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnwxhvdcc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtxkfqsa.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gnmcdzpbw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnvxnwyv.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkovbudl.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmklkigww.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbbsbsdw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiabbirb.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzsilymz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gribfyygz.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glnobmjlf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gearscbcl.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpwsngsv.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gsxivdazs.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/ggsqfqizd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggvqdjjaj.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gzpsbokxg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmqhwoahq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqxtulrz.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gxvhysikd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsntgvdhf.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbkwmrnr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gafsqntbs.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvypeksi.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/glryofine.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/glndbjjbz.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/glnxuywnd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glketlupy.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/glfyqqiij.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/grwxdzvhv.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqokzlzu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/guxfxzhwj.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gdxbqppzg.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gssbvtllu.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/grktxucvj.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuwkblib.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gelosxhih.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gpmadminj.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmuaggwx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gelymyidk.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyhvzjrl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gdumvxjzg.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gesxjswbd.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gacstjutt.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtretkzgm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtudwherh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gscpodony.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gxwfiswof.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqsnuolu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaeypzcd.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gdfkcbxpb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyynovnk.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ggkozeykj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypntwcvi.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/glwjceenn.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gqzdebfgt.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/giwuuawem.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gwttprmwn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxtzihxg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfrcyvlu.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gxzbqskyx.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhusqvbw.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/genuniwhs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkydvkhrs.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxhwwqns.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbddxauif.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gilptchxg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbgkrsci.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuszxhzi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijsnfwva.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqiqpfai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gupcqabzy.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/glgvynlqq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjscwihm.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gztdzwbhy.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/goiwdcgtv.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gkilcpjqs.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghddsvcwv.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuindbay.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gltccucsk.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwofezosx.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoctinfn.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/guyvfdijn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gavjkbotj.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gcojnokun.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggkrwscy.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/geezauqen.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gilkgzlic.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/goprpecek.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaokbnml.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwndhvxtw.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxhwpcbi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexqxdvjz.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcrfkfyk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/geeexjunr.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjgecika.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfshnixxl.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitilgcvk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwyilnrd.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gufxgwjph.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruipozja.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/geaimptkj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gpyddscey.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gfelzrenj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/glqfefrxs.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmkhcpyw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gzyqzcjzo.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gawsivpzq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gmpacupyl.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goovtigjk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/glduxynbj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzjnzzbh.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmvwimpl.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqbrexiq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gujyjiuwg.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gmtnhxhwx.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrjwstxl.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/ghzygmifg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gidggztff.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhhetuaq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkzfocoye.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gremjuszn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gksepyctb.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gskmykjwj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzuhdvmo.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwecdnrqi.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gljxorlvw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gkgnnahyw.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gmchjmusu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gfrrqhekn.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswlholhw.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gutabwscw.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/grxghggsx.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxmxdghbw.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gkztbyhqn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjtykhbl.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohkaxnka.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gledjeoia.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gzavprifr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gargghplp.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpwqtqbq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqfiidrtq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjkujkjq.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvzzxwte.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gqzoalhrm.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gceapzkun.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gvtkqoqmk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzweilulo.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gsemgetmb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gkopwxuhr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzwqlssqf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpznduryz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwhkspjgu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grwajahtg.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gebbvziki.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtejqestd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gawccpwwq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gisynkyoj.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gwobebuuk.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcktmxwii.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gqozfiyep.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmggitwzv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gqypxeicz.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaccxvgb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gquxyabep.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gogjwpntq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/ghebvvxjf.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupaiozez.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gfnvnmeya.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsmlsegt.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gcvczhqup.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/googvvfja.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/girmcolyv.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gfovehnuv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gtrckrunl.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/ggyojgicj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpjrtdbf.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiaxvhoy.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gzzuplzcy.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwjqqhwd.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuqucjxl.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/ggorsnoak.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmxvcnax.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqobuaczk.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gkpsoeklu.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gusbuowti.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gozbfnhtw.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gagojykvm.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gmmgholpl.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gqejtvrft.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmgslotm.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/ggmwomhhb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gtfjvvlru.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxikeosy.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gjubatech.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gwopyzhwt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gkshmdfgo.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glzyzcutt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/glliylajh.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwshjkaus.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gcotebviu.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/genmhrxoo.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwsysgoi.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gpepaojwv.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gselxekgf.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/grkqehxtf.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgdoaxjc.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdhpkgze.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggopthyhi.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gwwznzanr.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghruwdode.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gbmeliuoh.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdtxdzzf.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gubmtrpeh.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gtrvoikrh.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwiwfcdle.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcturqhbr.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gvlgymrnz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzoowhcx.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gglnqzxyx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gexnuxfvk.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaibibqqz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzprqxlzd.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvacfniat.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gihrdfzag.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gipbtmqog.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbzvpjie.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhimuvrk.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqbpftjd.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhsxtzvc.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdygimhe.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxbxiewh.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzbdooap.sHtML


<!-- 参考信息 -->