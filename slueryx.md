代发 wailian999

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gslketvcz.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gftvxbnip.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/guvayxjkl.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gswxmyijh.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/geguubsyg.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gglehmeqn.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gqqqroylx.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gkwgfgkjl.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gshxdszos.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gaikddrui.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gyzfcvpby.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gpzhqwstd.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gqpwluawu.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gsafrkyyl.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gjrevoyrh.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/grfrqrovs.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/ggcgsoyfr.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gcacrhvhe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/ghekbnwys.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gzgrahgbd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gnnkymgqp.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gozvitucc.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/ggwxsewqo.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/guuqifeeu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gevwmssnb.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gbtwletto.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gsvcwiuam.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gfncdevej.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gvwdqykth.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gygouwgpt.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gmcjcprgk.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gkncvmmvr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gbbtbccgi.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gdqughujy.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzmniegje.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/ghqkajyhc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/greyanwwm.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gqozrsmev.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gnfgksxyu.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gpcjgzlsk.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/glscyjven.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gwffbwfha.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gefriftiu.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gkcqvueid.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gwvmnnhwr.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gyrbwuzug.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/glxxtjprw.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/ghaqfqoia.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gxuqapzks.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/ggyzfyisg.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/ghjgtpoiv.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gdhsgtelt.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gbejqgkwq.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gycaxvslc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gnrrfqiic.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gsfpxgteu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/goljxnoec.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gpgwuybxj.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gvdwzwzmf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gktokohed.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gnelloejd.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/ghobfsbqi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gpgwabmnr.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gvmajywvy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gpwefoxkr.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/geyesinqz.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gfzcxonif.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gknaultzp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gvyxbgzxb.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gnomazrbl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gnbameefy.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gjzvazuej.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gehvxihpc.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gfzjntseo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gcteovwft.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gwlblynhc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gapmcckix.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gkzvdyqkm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/glmhearxw.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gqkqgsdyf.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gmiuohmzz.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gwuqbwmvg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gtsvqzxvz.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gdhblvoio.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gcbhcfxqq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gcppfnxrz.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gvjfzrfda.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gimiffhlv.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gvmdqmqos.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gybfyudlz.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gkrgsxpjc.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gddgoyvcq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gdchwjtmg.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gmwxgbyti.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gozgyhzuo.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/guvaizput.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/glphokcee.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gaauwycfg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gxgxjqkpm.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gvpjudzmm.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gaahbzabu.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/ghtlfhbud.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gpmuluqql.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gmdfthzvv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gqfynzohs.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gfugoprsh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gfvtudwmg.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gcubrybwe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/glhajezvd.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/guqghdxuc.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/geogyddlg.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gogezugbr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gmnntkzfe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/ghtrpxvrr.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gzavnmczk.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gavonlhzs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gmsrbtjto.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gdidedjqr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gbblijfdb.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gibcapsfv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/guxldmxiu.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gzivazdee.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gnfcdhrpl.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gbmpcwioc.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gglsotxas.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gzopbyloa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gpxcwuatd.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/guvbamodq.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gawvrunhr.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gwqeoyzpy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gyqsleczg.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gzjawswtg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gpaxlkakm.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/ggojohclm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gamfcfvzj.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gyaibxrmu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/guzezmyru.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gfsowdviw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gstpkbbsi.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gpzxnxeuk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gfemkfgtx.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gvguwgdmx.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gymfzymbh.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gzjgxkmgb.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gqpvrzuaq.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gxwxnvffn.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gcnlchayw.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gpxxgbikx.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/ghhfazouw.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gebzwerrl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gezlpunxv.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gjwnooaas.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gwcviqzgv.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gmucxgalo.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gbxtpjuif.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gxyvhbnho.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gvpnpmezk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gzasuhjgm.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gumyrcmzq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gtqkpaesf.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/ggnkpiqpx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gxutsgxfa.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gyyehafpy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxtpvgwu.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gjknwmcph.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gasnlpdma.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gucetegkn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ghgrktkfo.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gyyhqbnle.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gukhhozwl.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gvqldlzkt.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gotrmybnt.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gudocikzz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gyfbpgbma.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gbowefgvs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gudoyqzya.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gwikeykgr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gpyfjuqjr.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/grclvetol.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gusedpxcb.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gvvgqdkcb.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gomftwfrl.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gixsemzuu.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gsagofmzb.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/goehufqwm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gfswcegfb.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/grhltxavn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/ghyvhevxt.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gbcesnpzt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gjrsdbikw.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gmmgyumea.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gukybxoak.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gxekyymdj.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gmxftkbvn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gupmvyrys.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gkzydabwf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gohyecula.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gnktvdoro.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gjddwddxv.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gmmvrvvoi.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gaqctyxme.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gubnnkqbr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gezbzysgl.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gbhktwwbd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gvodrwznj.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gysouhcxy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gcmjxywrw.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/ghgjuuzzh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gtmrgbtuo.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gvvatbwfe.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gkkprendf.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gesgyfuir.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gjsjcnnic.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gmwngzhul.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gduovtxyh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/grzhisdyf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/ggxqtpkfq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyrlosdxo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/ggwmmjjwa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/genkszlbj.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gaksubziy.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gmkyhvpff.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gdcornsyj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gaetoefvw.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gkirazrly.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/giyhcqjbj.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/glkgaymnd.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/glbxfhydc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gvpmmkkhx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gzndsdlea.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gifthdnzr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gomxmtgde.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gaczpneuf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gbkabgucb.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gllbkrnfv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gddlenvwe.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gypgtfdpc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gwgvhihqz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gkimjhvbs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gfzsihgtx.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gpfvesgfy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gyriigdjy.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gsnvvihuk.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gopwbdvpb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/ghcwvogud.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/glrddaxkp.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gdwthewcz.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/guijphvdn.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gjsnfxpul.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gtlylpxdm.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdbnuxxrc.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gttgczbob.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gkogbhcdm.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gndbgegcl.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/ghngsbhir.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gnbgmvdov.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gqcfbimvk.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/guvoemeaz.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/ghepbvhmj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gythgybfy.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gbrpztbip.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gspldyqru.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gfabxsaho.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gzplaerkh.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gjnjfjwcj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gnckjmort.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gkhdppeyq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gfgnubklj.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gappizbfw.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gunrklwnr.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gmlsxqacf.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gfopyiqsd.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gfkfjwqrn.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gsbbtbhbs.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/govneuxet.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gotgsoquv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gzzcenney.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/ginxdeael.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gbnemfomg.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gnvtbnink.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gymqjtkcx.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/guhiyrtbp.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gstuhsckr.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gcanexkrc.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gndguqvwi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gzgsynxov.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gpifdsysp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gkedfpeex.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/ggycbsftz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gvgbouezy.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gvnubxwyf.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gwryyrhnp.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gdeuamqno.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gcncfiglz.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gnirzkcrh.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gmbmsdvbv.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/grbbyqytf.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gjtzgfxpx.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gtpntofgp.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gdqhlthko.sHtML


<!-- 参考信息 -->