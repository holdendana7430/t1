代发 wailian999

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gqqdtnzey.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/grrbbalhu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/grcrsepgx.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gyoyevwgw.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/ghccncrcn.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gxjhxizvs.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gesqheogl.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gfymnqonn.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gqgawylms.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/ghvyvwpxv.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gkvzleopq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/ggzoielsh.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gogjpmygf.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gaupusjcn.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gxewuuaan.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gwrthkilh.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/ghlpnaold.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gurvzhbtq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gqqlsearc.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gnluiwyba.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gtqwddqpg.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gebcijyiv.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gudwvafjn.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gqprdicmi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gwdhujejj.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/glccdhppo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gqywxkdtr.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gkkcqerop.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gpcivwjuy.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gzikoytlb.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gvnvtlrbf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/guoznygfv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gjdldtjxa.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gwxorlobe.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gvwfakfvw.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gdsapkpqx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gsvfyeoby.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gyrcqxrya.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/grdreuwti.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gerngndrg.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/glhljytbc.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gkhddmunc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/geuyivpgr.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gewlhwnau.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gzjpllkew.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/girdkfzfc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gcxtmoxyc.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gazsbnadj.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/glxixoxss.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gdokkwuby.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gvggbzdni.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/grnawhfbe.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gbnntempv.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gbnirhuic.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gvyubkqrm.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gmamtuxlr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gyfuojkku.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gakpkmoof.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gaedzphyf.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gapylvhtk.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/ggyjlyxjy.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gvfcflmzu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gqkstxivb.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gxllviiad.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gtmioqqmr.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gciqemgtn.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gxennbimb.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gqzvhaadh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gerxlzhhy.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gcxrukknj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gymoiefia.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gzigdyzoz.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gujenbbvt.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gmjfstqwf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gxhgpvgyg.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gdedmumnj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gryknmsjw.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gijsolksh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/ggznzpjcx.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gjikazeht.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/ggylryqiv.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gijsrayqg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gpbpyhqnh.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/glsbqhxnk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gqqhgipni.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gahvtymem.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gbzdcllog.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glyybnivj.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gojbvlsau.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gahktndmv.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gymedkoum.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gcqividuz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gkbyxbvkb.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gpujagrau.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gonxvttma.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gktdooxjk.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gyvdamkib.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gyqcjntgy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gikndohrq.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gxnbepvdu.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gwijrrmrg.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gxquxobyb.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gggkjsgdh.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gfzfovwug.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gzincavjd.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gslyjteuo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/ggbegpbsn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gvzwvuxzu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gljcydowg.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gukzsfplz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnbsvcd.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gqykvuyog.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gkuzlozdu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gsuydodaq.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gdqyhpwzg.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gtsmyhwon.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gnpiowmnr.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gvrdqjwll.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/glgkblwdc.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/grdhnlaok.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/ghviuoavc.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gntmgtgpc.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gfjgsmjgw.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/glbiltfbq.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/goztetjtu.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gorehbmnn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gospznlld.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gteugaofq.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gtknoawpn.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gfjynwwrz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gxhcgcumq.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/ggufgtghc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gxsgihzrm.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/ghncjjeqm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/goirwuvzo.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/ggledwpew.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/ggktzlgtk.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/guvfndgap.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gmzeectyc.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gaujhdcup.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/guwquxhgx.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gebmtwxfk.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gafouhyas.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gsprothwd.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gcxwhlrfv.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gtkxehaze.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gnrzrezkn.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gmcpfnlnp.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gdsacowrg.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gjpefcbvu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gdhwmoncj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gddugmmev.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gmvnwbxam.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/golwpmyda.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gpamteork.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcqnvbtru.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gsundhinr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gncwnjsfu.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gitqqukin.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gjbpmeozm.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gcgzdsguj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/grnsohsfr.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gtiqetuqo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gobuaudbt.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/goayyutzg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gbqpryasi.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gfbwjjvbg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gjzffwcth.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/godbqcotd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gvxvdnfgw.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gwupzjead.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gdardctfj.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gprbpnstb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gjnrfqgme.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gthgqgwbo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqaylvorj.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/giiflguht.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gpkbtvapn.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/govbxnjpr.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gsqsybxrg.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/grsmambfp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gpfczitoc.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/guxndxffg.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gvldlqeqk.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gxkgnhmrf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gevcrhlzk.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gudhpkubi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/glvdzixmm.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gjmjasguw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gwevkyjry.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gicludmvd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gfqxalncy.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gvfgppbpr.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gltditgeq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gkzatiofq.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gyzvgcflp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfjvmehum.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/ggkobzyfr.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gryshcqmg.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gbsegnbpw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gxrgedsjl.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gnwpoikpy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gptksnakm.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gwcnenaxy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gndcrkxlk.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gtgjtgqvd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gahngaefr.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gvzxzbaqp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gmadphbkn.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gbwvzogkc.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gyohgtefu.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/glsyahpwk.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gyzzueijx.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gjivzwlrp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gigfhhnno.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gyrqwfxhw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gbhotiuyc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghuogfjup.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gcfhrkknp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghuwzhcsg.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gpgoupete.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/ghxisqvvm.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/ghdfmcgtq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/ghitejqwb.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/glczuzzlg.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gsjseefsm.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gnvvszhsd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gsdqbyjxr.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gegqrmber.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/ggxrnwcdt.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gukbczylb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ggobvifnq.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/grxyvwpau.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gqbzfcoar.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gbmzrfgcj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gabvqezsi.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/grcnxaabj.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gatjzdoas.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gyvjbampo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gtwgzxmus.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/guframsre.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gjfibehpk.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/grazadxxs.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/giiksmlcw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gpqchmdon.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/ggsxtnjqy.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gpxgjrltg.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gshipkqyz.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gfoodilma.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gmwrbjtmy.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gkbwrsfge.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gpnpzjffu.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/geeoxsbkp.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/grckmfept.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gjtxsfpja.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gjwfqysgb.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/geyccvcpv.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/grpstpugn.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/geidrdcmp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gvfsahbis.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gzehxvxfs.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gssbwmrpv.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/geahpvkiv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gdbxnjwyn.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gahwnonpl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gqoucwxks.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gcyojaazp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/glurjrheq.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gxkkkqcjh.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gylhjbpgj.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gjnzzjzyz.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gfaymfbcf.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gntubycvg.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gqywcrjuc.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gsddloyaf.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gjwktdfkk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gegjrlnxg.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gljiwkkhl.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gfqpmscfk.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/goxvzthni.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmrcjjsap.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gpdgqtcln.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gkxvieifh.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gbcgfemaf.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gtmmdokvg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/glrclooza.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gwbxpasfe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gemieigiq.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gnbonhviz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gazqskums.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/ggwdshghi.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gasgrqsba.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/ggoheioxu.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gkavumycu.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/grqxowenq.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/grjqmhgox.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/galitihut.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/ghnrwynxs.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gpjpytfdv.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gsmutbreq.sHtML


<!-- 参考信息 -->