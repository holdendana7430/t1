代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwegcfkmm.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/glwtthndn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gkncazlpf.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvtpvuqgb.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gshcffaiq.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrjlqvbn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gvajzrpki.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gktfyrsie.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gumpqikkx.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gukljcttl.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyjmvzts.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gonlbbbwk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/glfuctyop.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gyitsfpxp.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwwgrvmue.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glhocsyda.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyyulnca.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/geqxmpdmx.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfevrzsp.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gnouyeqtk.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gmlbszpjt.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/giyiuxenu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gczkmgacn.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmbawfxk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnklrjfgj.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhidstvi.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcutrzjar.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfsogbinj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gehaexnyr.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawmuljtq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkicuqzoo.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/guslkujzo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gdywnaisp.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/giifbodqp.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gizdjajbb.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfohstgp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjvppznd.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnelzrdhu.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhbcdwgf.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gbldfxnax.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gjstrkrya.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/grxbscikw.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilruqkaj.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gbhqbmser.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/guqwyxxqw.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gotswqrct.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gextbmsjc.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/glpgcijeh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gglzkxymf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfuertmv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gyogwuhzl.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/geskcfund.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvzwudjl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gowaxviyb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/glznptssk.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/glpspffhi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtabfumvd.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gfrjbtyiq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gapxmvujg.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gzeijptcb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzdplamr.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gpipssyen.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gyydgyuxt.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtisyqkmo.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gruqkofou.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/godyzayhe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrjxaafp.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeoxiszi.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/glgutiigk.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gqulzzdru.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gbjsxxbwt.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfxlbulw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gixgrybqc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmcqgjbz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqbvcltn.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gcbvdasyp.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/glqfsmkzb.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganuruvzr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gejjslvcj.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gaahxxmue.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gtriakrjv.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gabikqdqo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gngbearmv.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gcqvtkvny.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gcqvmgsqj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojfnxpzw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gotskodhp.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcwuueol.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwkzcoqus.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gjyczresp.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gfjvzadtk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtftweeaq.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/guhjwdrhu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcryfqbns.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsvoamxl.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybkaahgg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtllphqox.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbyedrxk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwqbnpwj.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkssolbzf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/giqyjnmhe.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gxpnvbqme.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gkxbqpxzb.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwymkfvs.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gheegvhaw.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gzimuhntd.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gestwgppd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqqkwfxu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkedwgyzv.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/govxfnqxk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/ghtcacfxi.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gijotkhzc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzphosdz.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gtctbrbpg.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvavyavaj.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcodkjzoy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gtyemxnhj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gushwiynu.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gtoogbiop.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guviykdrm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gviznmzag.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghacsrosb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrqeoroo.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gbdllrqou.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbphviou.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/ghyfjgxbu.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkoletdu.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/guuxnkkod.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gblfvsdex.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gucapggci.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/grqavtfrl.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/giliiyyjb.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gidfsnukj.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/glbjfvzzs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gubiyvzey.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gzagrhxmt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/grliqukon.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gmrplosle.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlykaltj.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gcztqaoqx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpspllxtj.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gpoxrmcac.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gfttrkmye.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhflmcqm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzgoqmqa.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpghcclu.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/ggakmypqh.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gmjbdzsev.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/goahoazgr.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkpweolr.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gehpyxryv.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrcoplng.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmuemele.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwthrcba.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gxtbcvqqn.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gquairkbl.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gupnqdxvc.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gerwkydgd.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gaavmtquv.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqenkptiu.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gzgvzjqtq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geqnrlzfb.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtdllobb.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/grfnodrld.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gynewwsls.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garioetji.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwsgpkzy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gllqdukdk.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbxzplvt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvesoqcu.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gxaivxlyh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gymneaenm.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojlazwex.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gzlfotbfw.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmwecifg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjqhplna.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gceemflhm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gpzqcucox.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gngephdll.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoktqssr.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsazkngju.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhxeylpb.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grijkfefb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqpywnev.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbqjnpps.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/guyzecobh.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gcbogkewk.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwctajre.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqnbolmw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gwqulfpxf.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/ggpcdrewq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdwvcuafr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gnzrzuhwc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkfvkhirq.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnctpyhew.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gdxcaagzk.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjjlwitt.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmnewuma.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/genaklxys.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqzlucuz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbspndgc.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gnpwejfva.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gmwkpmquq.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvtqufpz.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gubzxorfc.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmgkurmx.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gdreflktq.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gbkepczbf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gitfwcktx.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gettapftn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gualpahxh.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gueksylqt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwvfwnpq.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gbjjoxklb.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ghyajfcev.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/garmubovv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqltbsma.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gkppqjilj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gkkdcwldo.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gkntmnfey.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfsxattw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gabjzeezd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcmsiywx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/geulkjvzt.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdarfbkj.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/graxiiecf.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqsbzruf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcphpjqx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gttsharwg.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gudezkzcm.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/grfkiffzf.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/ghavbvxaz.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/ggyobksjz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gxnztawsd.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyokzuyf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtupfmtqj.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/geryhgvqb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gdoslcjxp.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxyaftzp.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gpwtdilta.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjhcinidd.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/ggvwjlejo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgcklaal.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrjkqygd.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrnvfabp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/ghsfedget.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmpsilit.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayqllxmu.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gffpyqlzp.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/ghhtkzdwn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzqjghki.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/ggxbntqjl.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/ghdthabga.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gjmnpuxei.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugpwjluv.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gfgdltynt.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gkkauubgo.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfvzwaur.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwtvpvfu.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/greqxaiua.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gspnziyxz.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gogfbiatw.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gwjavftwx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkkyvahu.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilvqunwg.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gcgdauwic.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gscqwvjoh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gndgznxbb.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gsiunmkir.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/guopijjzr.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwngrbox.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxrjkvog.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/glicovjbp.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcvvhogh.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gfeggwzxr.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gintdhurg.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gpsuywynv.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gmioqanul.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gsxcaecrg.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gaykfthzw.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gahexwdbs.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrtwscbr.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gksqocmyq.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gkranwjya.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmsezctw.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuzzrxbe.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgcvnerz.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzdenmwq.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gxkzchbmb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/ggbihwegn.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gogbqslov.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gihioqnqy.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gmkwezngp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gbslisexg.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/giupqypxw.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/goujztfkg.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwtgfioe.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gfhprxoed.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrdqwzcv.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflqqufds.sHtML


<!-- 参考信息 -->