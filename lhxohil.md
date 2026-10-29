代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gzzkeyonj.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gcqvoibzp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/govzavbdi.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/ggtsbkdnf.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/grktogvtg.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gyprksyeu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/ggkdickgw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gzvzmxmzt.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gxbcsjyuh.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gadfztvdb.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gcoonfniq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gkxirztfy.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gwaieqshz.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gtudakogw.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gsyjczdtt.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gxrruofpp.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gwvgtdfjj.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gwzfutmmg.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gwbydjxxv.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gluuagnsu.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gvkplxoxc.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gzsfzvkht.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gfsvivigv.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gsyvfojsz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gyxqcmxlw.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gfnoopyla.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gmrwgqqoq.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gupafissw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gdmmqkxst.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gwkvmqvfs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqzrxsohj.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/ggplaqzbi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gfnnjwcyn.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gkdvofjvl.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gwxewwlmh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gpavrifnp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gykvxnfic.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gvbhorhps.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gpgzqyurn.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gxesqjvaa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gzssrnoqr.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gofmwlmba.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gmyzmqagk.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gldxdybtq.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/ggeerpmfu.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/grnbznhlm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gzcbsqbkz.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gzqmzfuea.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gxumifpeq.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gmovpqkho.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gnrcvefph.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gaeewcvlf.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gmlidlwqn.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gjmiianuw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gvouaizgk.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gyjitlugw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gymfplwpq.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gpqsfvbix.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gabrilimz.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gnkezftof.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gpmzzjphd.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gvhmitzyj.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gdwxshpgj.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gcfwfdhnf.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/grggkajpj.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gdnjsfuhm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gzkqzcrya.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/ginofhiew.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gsgyxddhs.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gkrgcysfa.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gybyjgogt.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/goqurrltk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/ghjocmxmj.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/grdzrobtw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gyeollskc.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gtcqvphdx.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gnaiujkdr.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gqlkulnao.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gpdhspnir.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/ghlxdfnjd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gulqnvuoz.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gmotzwccn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/ggvuwkovu.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gzmxsilyd.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gpgeizkft.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gnoeplwgr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/glqpsnhje.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gczwqtsxa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gimkotwvr.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gsrdumpkv.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/ggsweturr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqingsocf.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gefdipsuf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gifdmhncl.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gymrqpuon.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gmwbzncew.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gtastuluy.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gtwoxtwar.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/ggdmsnsin.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gtxclviee.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gcpabwjrw.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gshggldeo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gfywhrxks.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/glbvvbqqc.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gejnqanqm.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/ghwtjrasg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gzvordtzl.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gibrpzhnv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gohotbqro.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gnchdwrcq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gxqankdja.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gmfxuwnqs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/ghvanbzsw.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gemekqmnh.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gfryavwww.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/glddocdct.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gusrnkfsi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gskyhlysf.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gsfnorxzz.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gjsksnvgr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gpytdrgks.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/grqwwrctg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gahvzmsup.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gnfavlsni.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gqjbasoxj.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gnljrmpbr.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gzlifqctb.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/girxkvgue.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gsfofxbxc.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/giiawqlzi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gqenuhuwy.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/ggeuzjpyk.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gfrgggikc.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gafbjcqvz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/ggeaeatrv.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gfwbrkslb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gvdyreasm.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gccmejatn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gxagwmsnn.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gsshkafyx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gtyddkazh.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gvuxqcymi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gnmlnldgh.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gcqysolsk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gogrchdak.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gusoyqptw.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gbfdnxdin.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/golfyvwok.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gmzfnkuem.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gkrjqizbc.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gmwqlhxlm.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gfrjzlbhh.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gxyzefqbd.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gbubyucjs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gglmwgbgd.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gyytgaczk.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gbmacaqgf.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gvmgacbgh.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gpxvgpuls.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gfdofhjoi.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gbdzyudrd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gtopkcffm.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gnjqisegg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gdlyjntvn.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/ghyhtkczj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gzjompyjd.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gjonnihjd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gyuehdvyw.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gmxyvmfon.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gtmwhglwd.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gvspzdogt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggobbobco.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gtefdtiqq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gfngfypba.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gphdwsvtq.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gehypzuyu.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gpwmmxrhu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gaqdblnpn.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gbqklyiph.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gvyxepgxb.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gkvfbdxsr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/grrhxfhts.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/glhpvuilk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gmntckgkr.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/giorcykmy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gamiimdro.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gkzlxjvjl.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gbkidkjeg.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gmcnuiquk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/grxdjbmzc.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/ggphjhvcs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gbragcfkn.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gjklgayix.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gjlfisokc.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gmulvdbno.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gwgvwbtng.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gdnbzcgfn.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gkxpqayzs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gdlbvdsyz.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/giccuhedi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/ggvwqcblj.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gxrmuosxr.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/grwbtdnwv.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gzbxxrlxf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gqzpfnnac.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gvhahcvju.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gaipfxoyi.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gnxkptzau.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gsettuvsf.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/globnsfhg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gcpkipqur.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gotucwphp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/galkwepai.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gektuxjmv.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gnhflrmwh.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gxskigjwd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gkibuvnxs.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gwgtvdqze.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gusxqblxd.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gebkvsgxp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gllarzeby.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gworcdubt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gdprauwxi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grzjqpbyh.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqetnpnfm.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gdotfmmjm.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggatyfuow.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gyysevfpf.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gtlnjiqzq.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/glhqexwhk.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gzclrjved.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gbewbmvqz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gkenrczmo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/ggbeekxsi.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gfczjhxjk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/ghwrxyott.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gqjcjyjml.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gfhevumym.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/glrsbnckh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gunatvrhz.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gsjgyrjnq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gbyxgizii.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gvfcstqfb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gxapdqlki.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gkosneimu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gmljoyfpb.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gdldyndhd.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gzoztiaej.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gyucjeeno.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gcwwmikvs.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gavwvphna.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gacbwurza.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gavdsietn.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gylhetqiq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/guoyilnqu.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gikywfksm.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gdoumiusx.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/ggdoboakk.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gvdeyoeqn.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gxuclvnlw.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gdkxzgwab.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gsdtklrel.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/ghszifzea.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gyzommvzs.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gwacgosrg.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gufqwfeqo.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/ggmvianvh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gawsohwml.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gavlsrrhv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gdxpjvrfs.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gflntwxgw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/glbiiqdpx.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gxldhmdiv.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gkxktwcmf.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/geqqxumwa.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gjtykrule.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gtaqkxdeo.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gzdmeyovu.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/ggacudcja.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gqiobaogm.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gulyzmiln.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gereaseaa.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gpwbhzrds.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/guhdbcyiq.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/glibjurvv.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gbaoihuew.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gukuydovf.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gvhjdgqss.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gskgbtizk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/glzktyhbw.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gfaziicoc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gxlvgofsg.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/ghzzwdshp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/ghxemqlie.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gvavakgzq.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/giemrftaw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gncjydiow.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gtidwfhvf.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gcsaccmuz.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gtjkuqinp.sHtML


<!-- 参考信息 -->