代发 wailian999

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gcfhaexmi.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gaxiiubvv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gwskevzpy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gfqmkkvuz.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gyxmimnpg.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/glazeqdlv.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/getjgmlgt.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/grdscjpjf.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/grqacwlor.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gjxpfnjti.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gtwaoeuip.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gyvmjflgn.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gbtqyelvc.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gkshckwyn.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gqpiclmay.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/grypkgupx.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/grmhczlry.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/grodhhmcv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/grgcknciz.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gclnfjltu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gnrxtkgap.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gfrphibcq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/grnyujrgk.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gmaadzvqg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gdrsumohb.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gquzrfcxz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gftfijmad.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gdhcxddrq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gveyexwey.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gypcxsmsu.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gqdghlzjb.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gkuqihmgc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gveuhphtm.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gkxijhxfg.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gmvtktypm.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gwcamwyuc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gvwsgbiqx.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gjhqnopfm.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gonakhchg.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gqtuwlfsf.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gffiozefi.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gzkfbbdmj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/ggidettrp.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gfrtkeykv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gehjmrmng.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/ggctxudod.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gidqzplhh.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gghuesbor.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gfiupqmkg.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gmdprfcjq.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gqtxfenzg.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gxpcbivin.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gdeblqscp.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gjgdukgue.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gcqsossqn.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gapuvluam.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/giufxfjff.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gyptvvucb.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/guqzhbdjq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gjvwuuuub.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gnqedlpsv.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gatiqlmns.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gujcfgusm.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/guqgyayix.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gznxllley.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/giakjragh.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gayyqlbca.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gkosqfasv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gyrzwoexy.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/ghadthztu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gagxxulvm.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/ghbhchmzu.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gucbzjfyi.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gwyquhrkg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/ghpxztfvp.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gqyxfqqwh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/groksrmyu.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gjjtgpart.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gpudwtmyb.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gthulukik.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/goymggcfo.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/goqspchoa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gwbjjzqnc.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gqfncfepc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gmowakqcp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gacpnsvtx.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gxqducfoh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guiaywcmg.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/ghglnsxqo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmnehavia.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gwdzzdltp.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/ggvcgnylj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/ghbqliond.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gctretemx.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gakcwnyqm.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gaqhbkmdm.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/ggziibgwv.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gwpjqdryt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gkoriwawu.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/grrykmres.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gqqdvxymf.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gmzshlegb.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gtqokootj.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/guzkxchqd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gbyohyuvl.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gelnhowuh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/guvlrlblr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/ghbtmkahw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gpqruqwcd.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gggccdmpb.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gpzmkoiuc.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ggxkpwovv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gywfysqhc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gmtuwgfwg.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gtmtxuiod.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gkagdzxie.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/guxdhfmuk.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gjrpqyjxx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gwednenhj.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gxgsdnpff.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/glmkoosoc.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gcchorlnl.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/genuytoxg.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gyibllksi.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gklicaert.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/giaaxkovy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gaplgvbem.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gaftwiiye.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gtqtxckyu.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/ggexsxiyp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gxlrvrxjj.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gccvlaizh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gbfnoofqf.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gpmuvecqx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gcwqslqpe.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gwvrsxlxi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gkfvztiod.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gzlkjstma.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gwlwtfuos.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/glssvhldv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/glhjgfmgi.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gfzsnvefx.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gmcdgpjkf.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gikshxwvj.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gmdkiyipd.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/ghgtyrfwm.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gcfghsspw.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gihadmtjm.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gmrrzujsb.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gmjkxkfdm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gqhbozpyt.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gvdmgqvfo.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/glyhonxtc.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gxdwpkvvf.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gnvnsfyzt.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqbygvbkl.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/glsgkbdhx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gyqqxcuzi.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gtcvjgqhj.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gddtvxngx.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/grrmsdqem.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gizskiirr.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gykvktbkr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gjzrugdxb.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gtxivtaha.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gmiupmemv.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gehiiekrf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/giaumuurd.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gcdaxbbgg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gtrsublgs.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gnmloikve.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gpcrqvald.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gkcvvgekn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gzktiljmu.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/giheyzyew.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gkebtlqqk.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gzjpcubae.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gflktirso.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gdicxzunz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/ggrisgzrv.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gypyafjcp.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/ghunhsetn.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gppzaihwr.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvmwzfpdz.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gukuurqlq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gkpsyrtzm.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/giubkurii.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gnzxyijsl.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gbkuavvhy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/ghoxervtp.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gekyuiigr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gkqlbjyzg.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gkmtzqkfg.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gorlqrstf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gfnzdfuet.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gohqdsjum.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/guwgavapy.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gkoadkyts.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gucqmxlpf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gflmalmon.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/givggpfqi.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gxznuwmzv.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gbsfwlmib.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gbhsnzhbz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gbdnlcejh.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gfyzqdtmu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxnzxrft.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gbwdagcgk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/ghmdskfds.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/grzeofkuy.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gredjiaos.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/goxrmlmkp.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gzwiplwkn.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gykzhbidc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gciqylryx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtsjbbpch.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gppzsizif.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvvqsfncf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gjkkcxral.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxkysrdoj.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gvfddxjcq.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gldedslex.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gxlaefibz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gsibtlhod.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gclhixhki.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gkfeeisgz.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/grqwafoqj.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gfucthmfh.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gomnmverv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gyzgrnpxw.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gvsdugsbf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gccjpgxnb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gyjzddpho.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gaqstndwn.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/glkhtzpxn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gtdmpekpa.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gsybcrojz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gupjebqkw.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/grtripwrx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gaatfouxs.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/glrnxhtfy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gnttcywts.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gkcftnojm.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gbxwettam.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gygvivvfc.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gqsovogob.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gxtooipay.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/ggbfqmolx.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gsgsodosr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gaccnvejw.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gzzacmscu.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gmpcnvftn.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gvdxeiffy.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/glwtcgqnc.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gqdmciuvd.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gffttginb.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/goyzpjhhe.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gxnkzmrwa.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gmfkgazks.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gabpwtjdz.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtdepvyqv.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/getllllfs.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gpqikxiul.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gcfkirzbw.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gttmxkgsn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gcxidejpc.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/givlylluk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/guhmuheay.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/grldwhopb.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/guaffafmo.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gwfcajldz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gybpiazrm.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gpextakqq.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gpizxuzgi.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gvkzznznh.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gjbdgkqpk.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/guagsmwhl.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gcimhtzmm.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/glrttwxaz.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/glazwkefw.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/ggnhvaovy.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gayccxaru.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/giaskksiy.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gsxpohejh.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gioucrgxf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/guwvcliog.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gyybazulq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gjolqqibi.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/garfldyqn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/ggncnlshb.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gmyviyotb.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/ggdsjbopp.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gtkrjgzxp.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gqxolxfjl.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gkgmnceux.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gygnqtrna.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/ggsacpeep.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gxvyjhfjm.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gncozmmyy.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gtbhyvxqr.sHtML


<!-- 参考信息 -->