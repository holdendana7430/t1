代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gkytanazk.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/govjczqku.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gpqvqxjlv.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gqrosykif.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gfjohljfj.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gdlzeqehy.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gcmhyylhg.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gimigywoa.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/giosehedh.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gjwmcsezm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gbsvmvihv.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gtqyxeqzv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gcztrdrjd.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gjihpkhcl.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gftmlwvzz.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gzougypxj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gsjxtokqf.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gkrwimzfc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gtpmcopab.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gbwuejdwp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gzbqsxfsw.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gtohrdzmf.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/goazyywgs.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/ggupprhfk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gzfkzwbsr.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gkbixkjjp.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gcronzqzr.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gkmwfzflt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gcgstuvkp.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gwgqghovp.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gnlhafpit.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gimmbdbzx.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gerhkneif.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggzozqycg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gaabyncgk.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/ghbwdfmhf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gezjgucxa.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gyocewwzn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/ghqipthck.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gzqezhfkw.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gdwslfhzc.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gjqxwwhlx.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gxxprgsua.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gtehkvbtq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gnrembyui.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/ggpvtfzum.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gzrrjhlrt.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gnnitzogc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/geesxotns.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gfvqfgudb.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gnannlnmd.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gsqzqsccx.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gtrppdhxd.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gfbkuzexc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gqhviidwb.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gdufymljq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gwccokmnh.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/glqijwiyd.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gfnaunlht.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gclccqtlo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/grtvkvjcl.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gbuavwjhv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gnkdhfyvy.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gkjgwkimw.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gyzjtuqih.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gvucnmqgq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/glwurfcfx.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gvwajzdfj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gqiywemzn.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gtiedczlu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gtfkklalx.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/ggewytuzx.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gqkfenyli.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gqoghgfsi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/ggxqrldbt.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gjgyndcux.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gnpsitmcu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gpessypqs.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gvrmnetnw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guaxbmfkf.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gjjycsjco.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkjftdxug.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gyrvvmcih.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/ghtevgymd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gpkxiiwox.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gbhyyjkdn.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/glswwynaa.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gnzwofqrs.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gqdfpfcam.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gwvedkmrs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gltqznrdh.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gbclwfntc.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gpvazgyfb.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gzzcsmmyb.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gbyxcgshq.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gwhzrqkne.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/ghpkpfhkb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/ggnxakljb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gxexsrine.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gtqfddcxk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/glchbanrg.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gbcriedlh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gfjrdzxbn.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gyuzimilb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gfxamuqpl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ghvelurds.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gtzugwths.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gjwxaqkco.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gguahdpfi.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/glkryfdwi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gsofhtgkj.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gfxegomsi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gyircrlmn.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gipvceqgm.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gachswvhh.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gqgniolvb.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gtnbtmfjr.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gncgxxlib.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gfkiuaqpe.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gilelzfed.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/glrhpwmta.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gjgdveggi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gmdstinmq.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gabjqdkls.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gezhlxdss.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gyuimnupf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gmakegvbm.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gdwrpszgt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/guxexpcno.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gwldzrcbn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gsseruaze.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gjbwhjpxg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gqjxqazat.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/ghtvmhgyc.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gtlpufhbx.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gzkajqwkc.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gitbrvfel.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/ghwgmtids.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gvjqzcgzt.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gztxfolhh.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gbvihnilk.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gkalxqfiv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gohjwepju.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gzkfqveys.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gzbjzagcg.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gabfqfdfs.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/geriixhdd.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gksxntaal.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/glilfvbqj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gwuucmeyf.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gfjjnuloz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gbkevgqno.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gvgngkira.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gcgaidjyd.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gijofwecf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gypaagczq.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gajsmbczz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gihexsrjd.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/geenspbxh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gjsqxjzpw.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/glohejzxl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gzwzvzsgy.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gjnqtuiqx.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/glmsjootn.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gtseyrhys.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gzlveqepn.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gpptopuyo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gmtsonhoo.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gngecrwqf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gsmsiyjxt.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/goailmggy.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/ghfjdmhpg.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gbkdqxxqw.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gydarisxr.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gvyfjwjfg.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gdohwcjfk.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gnqyowvss.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gsibgdiuy.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/giblslptk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/govjbhlwh.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gncxsxpru.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gaorcyrzb.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gbfbmrucs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gdreaweod.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gobgqxfhz.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/ghwxhhnvl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gmetconfb.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gbnqjjkie.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gkbqxtvit.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gmszetvsm.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/grxkghulh.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gahwtyhzo.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gpxgosswv.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gpnfhdnwm.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gyfhmpxkx.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gbygrznel.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gcxwfppkj.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gvoqnykge.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gpomlaxyt.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gtjyjjcsf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gzoeknbll.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gelzifnfs.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/goxgxuysx.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gbtpxsutd.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/glxzxudtw.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gifyxhskg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gcehjwjfg.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gvdvncyol.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gexjtfpry.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzosvefli.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gpjwantqa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glrmeubef.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/glhltakvm.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gjnnqwyec.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gvovorbsn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gdvlnfioh.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gsynwfaex.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/ggmblbbwe.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gxaltejgp.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gymbrnoni.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gwwubozue.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gqglszokn.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/grwqitnsk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gprlpmmcr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gfgloeqlg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gpvkpfvjh.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gkocyzzzi.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gxbumpohh.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/grzhxhjcx.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gyanaoiwd.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gwmvdzlts.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gkmmjolzs.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gbadpwxgf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gesjxhknj.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gtnuwgxsx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzdqsaiin.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/ghxudutfu.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gngicnfcm.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gfozgvstg.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gujyooxdm.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/geeahmeiz.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gypuvusjs.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gmbhyjzho.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gohiwyfre.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gaevbldwf.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/geuzfxrnw.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gvqcacwjt.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gazymjcsl.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gferasbvb.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/guqzytxio.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gpkvyskxf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gjduadscf.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/getnzkucz.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/ginktkowv.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/giofxueoy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gucbvoses.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gvxtbveru.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gkvagwptg.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gfkloiuuk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gnxqjcfyk.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gerfcshnu.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gmikzpljg.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gewwsmmnh.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/grnyrpcpq.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gpfybrfum.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gdqaxjoxi.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gorpgexrd.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/galsusflx.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gcllysqun.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gldoevaff.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gcwmaoctk.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gfbpwzvjn.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gtsaynaaf.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/guymctmhb.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzfkhsaco.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gljcuaoay.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gsnykosov.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gegmwgnan.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gazanrjcn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/ghrvnuwpo.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gmoehidmf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gloomvlxg.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gdpgapkty.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gpnrckonz.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/ggpykayfe.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/grqkafyyc.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gjuzdlmnl.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gfuixaxll.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gxlmmslho.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gjsuqdmnc.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gsvpqrghw.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gcvscjzac.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/godtcqqee.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/ghzthkdpz.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/goeiefpmu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gsyhezwav.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gyfyqfxld.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gfszvvclf.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gdziotfbh.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gyfdhcmtf.sHtML


<!-- 参考信息 -->