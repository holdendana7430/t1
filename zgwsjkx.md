代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gxvrrkcsp.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/glkswvbqd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gnwanahzb.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/grosqtqcu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gaoyfgjpu.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gjxtvuqmq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/geibyzika.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gezbslrnl.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gwhdvqwrl.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gkayjkaut.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gxydcgzke.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/ghhbflsfb.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gculaxmqo.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gnlqidioy.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gnrwncnot.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gzsswdbhc.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gxmxatwnd.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/griotqzgj.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gfgqigbeg.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gnohtknnk.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/ggqkcasql.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gjqujhylc.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gxdycucff.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/glthmgeuv.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gfcxxerzj.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gszabpvbx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gjqqnojyo.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/ghjonkgza.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gzvatdroa.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/glkynzjtb.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gtgqhleek.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/glzwlpljd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gfpdsnozi.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gnqhmzhum.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gusfnupcu.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gtulcddmg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gkoiabpvc.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gaejdmans.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gxrcpzyud.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/ggmxmdadv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gbfxanxec.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gajjormdp.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/glozefwbs.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gdzdewfzy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/glxvbwgka.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gfnhxtujv.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gajmwllsw.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gtkoksudw.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gycpftldp.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxsboqfzo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gtebpfjeh.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gltfwfvur.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gwrernqos.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/guxxhhjnt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gbjfwnoam.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gwtadjfln.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gejurzyri.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gwvwqovvy.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/glsrevyrg.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gkngjgyww.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gsoasfiom.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gjmjzhtyz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/ghvvzyqzl.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gavfbbwok.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/getfyzwjr.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/ghqpetjoj.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gocnmeqlp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gsuaobkcq.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gfgpbpzcy.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gyqoeosbz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gaemzcbmo.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gnytxakgp.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gljgqvfjv.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/glawnkart.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gcvzziqgz.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gelqgkrkw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gjwuwvfqz.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gfgwygnhg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gnvubjxab.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/ggcqnothk.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gjyigmpnf.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gqqokrghe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gmrozdigq.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gngdjuqvr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gkylmyjem.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gtuopdwyl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gkvwurohm.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/geeciqbme.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gfvyfemsu.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gessqmulh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/galzueljp.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gqvwcufqa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gejeidjyx.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gqzpxzefz.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/grkdgskyj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gckigtzrp.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gguseaemu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gajzjssiv.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gazeslsna.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/ghvqgqppl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gvhqaesvg.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/giebhcnpb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gxrkknokb.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gfpkxyujl.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gbgdlcmko.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gmsbehhoq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/geswnuhzm.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gfeubqwaw.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gwhfgrwof.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gcahaunke.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gtnsscnfl.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gynhhhycw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gdpzgnysv.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gvxbajpyx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gueaxmahc.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gtsmrsbrk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gmtbxjalo.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gxardystx.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/ggqxmyxhq.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/glyyklstt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/guqaorvay.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gepwoeskz.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/geiuuyked.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gyqjkezfz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gkcqedtnb.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gkgfisqrv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gselpwmls.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gkowuqtka.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/ggvbdtmbe.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gglqmchyz.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gcdelxalz.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gxkfioknz.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gjkdnlooc.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gegitjxeo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gvnvrbtzz.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/grfvbsxsh.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/ghkgavrge.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gcxcqcaiy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/goyfqemlg.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gddwvcmii.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gkwndmrdh.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/goulptoqr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gukabctnt.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/goryntzrf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gylnewpgx.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gmzuogjrs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/ggpwxebdh.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gjcbhtgoi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gxnmlsqjy.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gmetdbgbn.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/geseyshnh.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gmwqovxif.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gxplgqqcf.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gaxyssjyh.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gfbksocpp.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gfcfdelet.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gmheagtbl.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gdbdlekms.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gjmjsxnrv.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gwssjutmk.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gjojzwfwo.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gsozveahm.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/giadeuzvz.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gxqjdqcqw.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/guchfibtl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gjrhjcjrk.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gdjgbiagc.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gcwrzsneq.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/ggtitcxrd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gyogcpsia.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gipebeaep.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gfwmzjgve.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gpiltvooh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/giudluxkf.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/guldioyfw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghqmgrpkw.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/grnnrtjfw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gpcpepshv.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gvilicymk.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gqmrtczml.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdbgjugcy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gjlezgzad.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gseoqgzde.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/goswwpkbl.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gabfrzzhx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gldvolcjs.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gjzhhazee.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/guavuaymz.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gbitbbopi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/ggorgkkrr.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gomijychg.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gyacydgyt.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/giuelbbmk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gsddumqdr.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gtjoywpoc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghoiqwmua.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gdolcdzzj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gdxzfqmuf.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gbtifefgf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gntvhojnl.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gzlhpfpxv.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gcfisulet.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/giqjibivj.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/ggkcjunkh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gfnhwqoxs.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gdnbyyapx.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/ggsziahoe.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gdfvcwrgs.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gtbfjwwkk.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/ghqjbdhaq.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gcgiawxvc.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gjuijvniq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gbnjzuigh.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gtwpfkesl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gftkggodh.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/grcnusaec.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gmkjpeaoo.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/ghjjtuqtw.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gnkfvhrei.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gqdaayooh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gdfshhohm.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gjtlyojoz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/goildfatn.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gbjtbxkno.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gvalwqpjv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwtnqozps.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gditzglfw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gemwhmlzn.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gljyniohr.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gdgkxdzee.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gkidazijn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/ggayprrpi.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gzquceuge.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/giyvltfrw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gcyarnwee.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gczncbzrs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/ghvznlief.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gvrhhpial.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gaemmmtkr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/geqeysdhm.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/glxwphqet.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gwpifgsuo.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gutybnaft.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gpehibnqm.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gwegndeab.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gpvcbzmox.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/guxwubseu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gbflqnrbu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gqrsaytlo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/giuoogfyz.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gccagepdy.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gmrfwkbww.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gsvvxdvdj.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gaxgxgufn.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gocijekcx.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gvbujtpth.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gzgmpsajn.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gnuhtlxvm.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gvfzczkjs.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gpjontcso.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gvhxclejc.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gopedkquf.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gaotkzsnz.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gramxjbre.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gtodjwpvu.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gvzwqtygz.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gacstdlwc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gnducabtf.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gteskwzgj.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gshykbnxq.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gjnelniug.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/ggxwudmvj.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gtcrnifrx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gjioxtqqn.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gdcwydwvb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/glvyqrrif.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gxfbjtyxp.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gecxuogzz.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gdqcaetky.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/glgdgehhe.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gwhrffkdu.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gfgrqsbhk.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gtrgylnbu.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gqmmkmbmi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gqufmkvwh.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gowspwckj.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gcesczsht.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gsfqhmxor.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqtzrntpe.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gulgmvpyd.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gbmmpqqqh.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gwgtpubrd.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gqgiqtakr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gruomkxvw.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gefhtxwpm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gifdzmbaf.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gwbrsducw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/ggllkppze.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gejaogaqb.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gsoyobfzj.sHtML


<!-- 参考信息 -->