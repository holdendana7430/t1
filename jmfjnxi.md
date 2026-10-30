代发 wailian999

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gsvnqnfjd.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gojzexzbd.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gpbucuanv.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/grficxikq.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gybipqgny.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gkydvflfm.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gxuybvpbe.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/grjukbzzl.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gnowqrasj.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gbmfrxedr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gqfepwkdc.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gwpvcpsoq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gygigllyh.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gjrgnihes.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gqxqzmoqs.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gqnolxmfe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gedjnlwza.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gevamyhwa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gkenwjvyp.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gjrmszzxw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gbsdxnmlc.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/giwqapiis.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/grktccztv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gvohbpaoo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gtbgwfkxt.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/grbmemwaw.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/ggkphwyre.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gwowxwwsg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gspyaefnr.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gwtdjyrhe.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gebeneljv.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/ggufeobzr.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gpuixbvid.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/grckzmdjh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gicinesfg.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gwcpkhojf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gfmguzjow.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gipkzglcu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gbxelbyfq.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gsalnchtb.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gwnrxfjyd.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gslkeitiw.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/grszsgozo.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/ggrfcdpqy.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gkvzmxfid.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gljxdpogw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gmyfcacye.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gwfjtbqro.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gqkfgovtm.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gwjburvgp.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/geprvuzgm.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gqepfxzmw.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/ggirbmqrn.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gjaphgvqu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/ghgdkrays.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gmyajkbut.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gdyicivjg.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gggjzsjwy.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gedjsfete.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gwrguushf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gdroniuyp.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/ggwmlnigp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gvlvhyavu.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/glbsfvdxh.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gkdbzwtox.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gwxrskjdk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwfwnybkv.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gtivahuqh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gojiaiwxf.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gnvrzoyky.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gyuvxbelh.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gxpzesqcc.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gnuxvdftg.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/ghtpgfxwa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gbvbtmmka.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gncikjxtj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gzdehyfmb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gsawckaau.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gguyetueg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzxvisbmq.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gsujnsakf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/givunlruw.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gsdqwjyvq.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gmzrnrnnf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gtiphoeaj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/ggmoamxbx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gxvevdisd.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gfjuqybpw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gmpzqcfjw.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gaznqgrdz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gcgtjyqsa.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gfhydcfgc.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gxyiloipk.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gxgafbqam.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gofclfjqy.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gcxxpxmvw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gzthxbong.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gvyghtitr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gyduvsgfw.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gdvjbgjfn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/granqhoed.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gyrdtgflx.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gyivcyrcz.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gjtocuuhf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gopyvbxux.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gqmrypgio.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gzujdmval.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gefadbiad.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gzcdmtxcr.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gtgymsuyb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gkwztshun.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gjktycznv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gmonbuqjn.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/guwbkabtv.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gxbfyulou.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/ghrgghyww.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gekfsewiy.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gjihfbekl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gkvirsqhi.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gernwfgsm.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gtesxjwej.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/ginvwyofx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gpumynidt.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gcdjafdol.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gncvgbxmp.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gvsyiyaeo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gmlpjtlhf.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gxoojhuvt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/grfwwguuo.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gctrgdvqh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gelhgbufo.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/grfugbict.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gcdwckysy.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gdrsyhepj.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/glwfdomet.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gdtoegwrp.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gwnhrjdzd.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gjowcfpma.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/giklcblse.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gyrnyivxo.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gbzttfzvr.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gjobmcwhk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gqxnevylo.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gkjswizxu.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gapycmlda.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/ggsslyvgk.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gxbyoodjz.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gglcuammu.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gkuyoatdz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gfyqivhie.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gozfdopnk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gcmhuvftv.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gomtucsxc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/grclrlbdz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gfflqratz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/ggypyymog.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gedklkxwc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gfjgdqszs.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gdgxwteiu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/getngefje.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gqhtzogcw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/glpsmzfjo.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gtgjuassq.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gaqcgzyie.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gsawczrft.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gblyrsnqg.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gkwobdnai.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gzswdnzdk.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/ghqyjtftk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/grazyaoxp.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gunhmzsui.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gslrahpqw.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gesdozejn.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gybjncybm.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/ggkubonzw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gbdbhvyhm.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gbqxfwulk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gwysixoma.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gnkqrdlnh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gwufhrohw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gwbyanzvl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gvsdkfemo.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/ggbbctagj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gyqixvztu.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/geirmokca.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/grpfiujrn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gvmklxnri.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gjxuwgvms.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gnnaojepk.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/ghrewwtnv.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gaigsqokv.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gqivkyzjg.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/guhmagxqa.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gnsntqucv.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/grcghoqvs.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gonxojoku.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gmqxedjki.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gfnnvcymg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/guqhtidmt.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gxoanagjq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/ghzifsjka.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gnqniwthn.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gxwrwzgxt.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gsqwkwilh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/glkwnfinb.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gvzmpfltq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gzhhyccve.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gupghcijd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gfgplkcwl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvxlxwobr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gjwzstdft.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gavlwdkpq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gryofmkjj.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gzmafuapb.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gdiefltuy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gshlnzdnl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gcgtigfig.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gbdhxgmak.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gmxmfyjbn.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gbohdabbx.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gpjahwduh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gpknlblys.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gnvhhyest.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gyzbhdnha.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gaxwhmtib.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gsxzxfbge.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gsersiblq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gtrksdmix.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gflzpjqhp.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gazeuiile.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gubzdhzmm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/guvfpobrt.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gelpcmudd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gyozgkfbr.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gkcikcrgs.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggjmwshxi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gvfmfjnlx.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gfpmomofp.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gxkjczqgj.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gaikyazmh.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gfifjfcra.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gxkwawvvl.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gycgkyggm.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/glqbbqvje.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gnfchjjok.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gvopxyasa.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gpvkulzyo.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gxbndczka.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gastlzkhm.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/ghbchyvju.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gtjcmenfj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/ggmprbryj.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gwmokskhs.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gyuxupssx.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gjetjauug.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gjsdgbxtz.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/geiwskuty.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gtmxzixqq.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gmgnprkxf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gzacugqmh.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gysjlbpoh.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhdmtfpy.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/ghcqvxhnz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gppisxnhd.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gqvvgdsyb.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gffcrbutv.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gsppjyurr.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gjaogoqih.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gpegnwouk.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gusfcgqcf.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gtnfldwar.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gmdaylmnw.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gabqlwjeh.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gngcelrbg.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gnowfvttv.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gsgirzpar.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/glmoxxhvb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gbgomchxg.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gcbztunnf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gzgeozdbe.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/giihuhqqc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gmgkzksku.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gnssybigk.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gsqhrsyxz.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/ghveuyrns.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gcnbtoyrg.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gpdmwiitw.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gblqltiwv.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gwthotdar.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gcovepfhb.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/ghmjvuubu.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gjuhedwet.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/ghevivmfm.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gkghcoccb.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gfnhidkwn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gzduviiyo.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/ghmnruqsw.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gduzkgprk.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gmxhdcpeq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gzuyeywjt.sHtML


<!-- 参考信息 -->