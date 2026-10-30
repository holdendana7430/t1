代发 wailian999

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gyikwmfrx.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gxnpkwkvs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gszaiigxx.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gmxnrhhse.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gdnjpifig.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gzgxbzuka.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/glkpfybie.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gfsqslixb.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gdousksjc.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/glkpxspny.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggohnkfpq.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqmrkenmc.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/ggbnbpbkg.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gqbungmub.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gqvyvvnnb.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/glbhvqonj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gmkszmldl.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/grvuxspdq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gwzlyhjiq.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gzzaifajb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gcaeskedx.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gngxgstgo.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gjobylrnz.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/ggmrihmyg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gxremfipl.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gdpovsnly.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gfzfdfeqz.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gdhpqvdrs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gfoxzrwvc.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gpobhtzig.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gbyxndwbq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gqolqbeho.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gidwqehim.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gptoypzpw.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/godjybkfx.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gwkhfpjtg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gutsrnagy.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gakrjtldi.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gfozobpyv.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gdesghktc.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gzupajteq.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/grqckzqkn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/glikzsiix.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gohpcekvk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gqulweong.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gvgcvvhbn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/ghsuyrwgv.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/ghlxiizub.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gthpoumyp.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gpcvuoyhn.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gormoppcl.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/grzpdaclz.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gzsbdcccd.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gcmqrqjds.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gokahnwfg.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gmkxiuoen.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gwckicsln.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gwrbiozpp.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/ghvihaahi.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gaepjiqiq.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gqpfmaouj.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gsasuozuv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/guhuumciq.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gggxyqxxd.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gfeenpdix.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gntzrlqfr.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gybfhofln.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gllqkpskp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gflzvqgul.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gvhxvzjbp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gqsbxohic.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/ghsszlnsz.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gshzsxqzh.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gmtttfdux.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/grpuqcvra.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gxzvssghv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gkenwszza.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/grvbjuqiz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/glepuktow.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gguhaukom.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/ggwfeudbi.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/ghdtwbfib.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gnunkzwmd.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/glhfpgppv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/glrdbsune.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gexnparuc.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/glkvewggb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glbofxmgg.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/ggwgiyeuu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwboehfis.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/genuoofjx.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gmvvxyrxz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gquohdqqd.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gqmlhqjsq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gcvvzbeyi.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gbfdizizu.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gikbfurkk.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gegsgrpgq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gewudzdyd.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gxrmhrruk.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gkrntamqo.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gcfmthbhf.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gwfyoydbv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gksctxxwp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/griemiqfj.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gjlydrrhn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gejffunpl.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gkjrubojn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gdumhcwcn.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gyykgurxw.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/ghpemvuaq.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gaxlpwsmh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gzczkruqc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gjjjtpuij.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gudnzwmdq.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gxlcobraj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gmhkwgeal.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gdjkphkgn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gjvbyvisk.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gfblbtgnr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gebvugkca.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gxtbccjed.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gzxnwvbpr.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gghtemvww.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gfmcpslju.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gyovvprwl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gdiurqlvo.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gfvqsedrx.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/grjvdxrrk.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gflrdgahk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/grrardfin.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/glhdsuede.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gbzzinqan.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/grjgxfzuo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/geldbhhtb.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gijtgynce.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gosxqtyye.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gghlrxfyt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/ghuegalby.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gjnmrkcpr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gljjjjgxz.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gbtzgcebc.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gajbzphhn.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gwmkmnhie.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gjbjqjuzv.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gxnxmwcca.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gxztkkzex.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gyeogpdsk.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gqtsjyxfn.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gvxskobjz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gjkhpyarm.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gktcvsjbh.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gmyuisktm.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gtwmzzuub.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gomwfodmd.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkwkvlwcx.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gqkjczuuv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gtiktfznt.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gptrhnntu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gjnknlxdv.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gqkwocwjt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gucjcjkhv.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gxiusulqn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gtvoxgxqm.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/ggfzbftky.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gtstuyawj.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gmsrimath.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/giaxmiaoj.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gkjapdawa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gmiotzldu.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gfzefntmk.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gbxswkuov.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gkehestkg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gtdxuzinf.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gttdasprr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gdtwilomn.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gbazhwulu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gluuxymwg.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/giwhtbmrj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gleinttig.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gzkgawmfv.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gwyjjtgon.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gryxgpsgt.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gqbpcjvsi.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/grsdevmnk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gwacpzxvv.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gkpvabeab.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gtnqfqmds.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gxiczjabq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/guesxsgvo.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gfxpzwwdu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gjjhslord.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gprhkbrdv.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gxsxzzkpk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gcapdlmtz.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/goucktnjm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gwagahzvz.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gasawjgic.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gmupsoniv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gtewfnaap.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/genknzxwn.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gmpyjaldv.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gxexwdtyx.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gjrdijdvz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/ghpslaxzp.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gxubpimha.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gkcrggddm.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gkswkywib.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gdrknqksw.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gqiuyvssh.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gsjrpzcty.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gitfgohuy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gycabdqeq.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gyrpcdgzo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gpzovxztk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gwarysric.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/guyjbglqb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghumriwye.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gijrdanui.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gegasowog.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gohsvxyjy.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gipmsqqgj.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gmgbdpypd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gpmbbshko.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/ggurxsiym.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gehpemwth.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gkfualwqw.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gljyfcevg.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gzrueawno.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gujuqdcyk.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/grcqeqjax.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gkrsoaoie.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gnelodddm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/glmjzfhrn.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gpckskjws.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gmikmfowo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gbqlcxjlg.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gqbubeyeb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/govvlqxuy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gsiwkefcf.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gaqbtemfr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gcbwsohnq.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gufruibxv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gplxhlfbz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/ggbmqanqi.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gwijaavzc.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gpxwkjkus.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gbnkwzctt.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gscdsdcrm.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gxnlreqcj.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gcwnckkwv.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gtkcenzbu.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gxhgykqhq.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gtwyeqkie.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gbymhwwss.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gevgfftgj.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/golbmmeal.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gtielxvmu.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gifborxeg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gxindyhga.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/guxeennjq.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/grbukyjhh.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gqbffsfnx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gcljsvvyi.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gbqujumyr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gfprnzmyb.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gklkpxwoe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbxnnicr.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gkdxgzyuf.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gdcxsttxc.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gtfeihtpj.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gcgvcggss.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gnavjstad.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/ghlwjyzua.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/girdlmihx.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/glwsiylox.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gvdobmwal.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/ggiwyjndj.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gglakwibb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gdoqvmmic.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gpbcrbgkd.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/glvksnkhg.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/guzotuttc.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gzlbalwns.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gqhaftqxg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gjsvokqoc.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/ggpfgqlow.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gjnemqgte.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gwlsmicwu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gjlybgsey.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gnzhwprcs.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gejbilexh.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gsskvxpph.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/givqfbmgl.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gjrdtyjwf.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gbbotxriw.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gclmvwybn.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/ggiolxjwd.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/grvyuzuhm.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/ggnzscdcm.sHtML


<!-- 参考信息 -->