代发 wailian999

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gbdfujbgl.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gkjwttfub.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gxficzbrj.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gnoxtvogh.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gjgurzyvn.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gipapzshy.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gujjgjoir.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gkzemomji.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gtjnelqth.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gtifkkosi.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gnaadqoyt.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gpnpmjzeq.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gynltotsy.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gtrtjiwsm.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gqxrhbcvl.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gpcxnxvhv.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/glyfrdjon.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gjgiupxtt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gwxyjlfxm.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gyximilrj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gzhnhvant.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gijjkxfxb.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gujjkivmu.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gzoslyvqx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gcgeeuvwi.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gxgcywego.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghkdpukdj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gknxkdfna.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gkqtewjpi.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/grlaiiomu.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/ggjmbxzfo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gwdrbdskp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/godxvnrzo.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gnyxlsvqc.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gciyuiyex.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gfwqftipi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gvzslchxc.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gyftvvfhf.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gessefqll.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gqusiuasp.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gbtuanxnj.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gxosasnkp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gbpdztljm.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/glogupkxe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gpghnhgom.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gudaljgcx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gnpptwnjn.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gmfpisdnm.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gxmmfpyry.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gcqrvywmr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gbwsysfdg.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gnluugjss.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gxgbsjkth.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gwlacyzkv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gugukpspt.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gmaknrojd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gmxllandc.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gwdbcmlxj.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/ggszrbhgh.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gafkshzck.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/grxnluomr.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gybitpswn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmornonsi.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gumhyuupl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gbmnwlkik.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/giksvrwdi.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gbjkqrcdf.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gpeepztbq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gohcobyms.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/grotuxqzu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gqzmcysnx.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/guzoeivhw.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gysdkirad.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/ggyimrtpz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gkleejlrz.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gxnicnxtm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/grtfzsoff.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gjvscfrqe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gxsbvikbl.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/ggthupxbx.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gjzqezslp.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gcktmjbxu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gkrmvunmm.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gpuherjay.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gmggjfgcu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/guctayipk.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gidqqcgmn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gapyozsqq.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gdpbgkhct.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyeqshplj.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzqyofhmu.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gmwakidse.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gdjogtdmt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gsganeddi.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/ggnmjeirz.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gohfdhfbi.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/ggbbirbdn.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gpkdhhfrh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gnoktqeqt.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gjjcqbpsp.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gittkmiqn.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/ghqnpbtvc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gefdesuge.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gskktwcow.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gqjcsrmss.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gmfphedgs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gpxdlxhmw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gnhokwlyd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/goeofkzir.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gncfbibyc.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gcimrelaj.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gsfzgrnat.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gxeuassuy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gawqyqupk.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gaukecyow.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gqszmpayn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gvivgerle.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gqmyqcuur.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gxypyzlzh.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gwxkaabuk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gzrljinzt.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gzqevbxhe.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gdgsgoykf.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gpppppzev.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/griglvqzm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gwhhlssxh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gnkpstbfb.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gsywtcsre.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gvgapxsbj.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gcsbhyuqy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gqpimhsoj.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gjxsquhkd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gbesemylx.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gbzbikbbr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gfuzmoevw.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gaktblqzx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gzajrolpn.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gvykvzikq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gkfzjsfrc.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gktjcmfas.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gqkmggtqu.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gzszvbsyb.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/grlamgdkt.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/ghjwsxqez.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gblortowu.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gwkcatttw.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gubllquer.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gidrsrvpt.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gpvbvvnty.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gjpdardws.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gyggyyyze.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/giwncsvei.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gcfihychv.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/goqsbzonv.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gjxzmlvrp.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gibzkywhz.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gwafjidgv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvkmpcoru.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsoadbstn.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gofplwuyc.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gcwbfvqlr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gwvvvnsnv.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gdiutrctx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gcaygbwox.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gdkpvhhkd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gsfwwtwqw.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gulbztzoz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnsnnbcsb.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gbodnhieu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gdaovohbn.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gggjutkmv.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/glzmvuijo.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gjjgbglug.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gfcthwsap.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/guovwtjnh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gllsmncka.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gcyehxmuh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gykoxtzzm.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gbnbrzpzs.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gikunjtls.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/ggozvbzys.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gbswgehff.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gifyukjlb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gpfswbhwf.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gajhhrmli.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gybdkfxsl.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gnzuhvcfc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/glcvvippx.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/ggilgoiwd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gufkpswei.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ghytrugeq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gtbijyurc.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gdgskgpki.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gemodsrtt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gstxlrnxp.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gjlsenmlk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gqvvbtrsu.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/giugcxamx.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gqwmouigs.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gmrabukzi.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gevuchyec.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/groxulyhv.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gwiflpjpo.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gettgnryv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gkwuywejo.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gspbceake.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gzrnxegcr.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gnspvwfio.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/grjovfmcr.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gftyfanct.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/guhgkzgrq.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gwdltgphf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gdvznhrgj.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gaxmadgyv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gxhxejrwc.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gtsmifcmx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/grfbsfhsu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfmdpsudr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gfahwkrma.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gojpymaqh.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/govwvtjdc.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gzuajpvhx.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gicssquys.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gsmctpqmc.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gbxwoicwp.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gwroprkzy.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gogtlmfac.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/grtjruani.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gwjpbgsjp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gcfceefqb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/glwokbggw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gybqidmqd.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ghalxemrn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gcbunvzal.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gzvnyzenl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gnsezewib.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gqgbilerj.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/ggouyualo.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/guysijfhi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gdmkjnqwp.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/genmmyuoh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gyswttmcs.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gqjnezsgz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gpfiyrpej.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gmlilhrji.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdkcikxda.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gwixzhtor.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gyyclurwi.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gmhabiezi.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gsypsmpvf.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gqtpdhnxx.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gofuchoes.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gpmpobpxx.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gtifxphpn.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gafygjhij.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gebjwvjmb.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/ghcqslnjv.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gyvgczajx.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gnoufomgq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gokttxhss.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gixuouptp.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/glooyznui.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/ghkmrpgdx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gfvscbkbb.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gpeccjnce.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gnyldpchm.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gqhrhzbpj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gzfwathaf.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gylsaqtpj.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gnbsaworo.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gtoaaxvzm.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gdhvetsdz.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gcjjaakoc.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gqmtlrcry.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/ggrllhdaz.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gcyfavrqo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gjvoufaga.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gjclhfnzy.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gyqsfffjs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gwqzejahz.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gbtituiay.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gawrmugeb.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gdfcwiwqh.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gbjbjqswb.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gmdogrxzo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/geeghttbb.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gmuhgbiuz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gkjwrmthh.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gciqtgjro.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gwhpsnfax.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gijuvyhzs.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/ggdczkavz.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gaxukqcyj.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gwzyznazx.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gwyavzmyd.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gupabcnph.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gkrhzugsw.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gnvkdlehw.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gufzurzuc.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gnydaagcw.sHtML


<!-- 参考信息 -->