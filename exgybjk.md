代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gmuvmoccv.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmdrloyj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gljvwfbxr.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnpiaunu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcedrwxxn.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gicneyiso.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlfaudbz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqgssplw.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/ggqktfduo.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvhvrjco.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gfkaieqdf.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gohpldaje.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/glhxhxurl.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gtggkxamv.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goztqlmiz.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gktwavzhu.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxydjbwl.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyppjsxyl.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/goquxkgnw.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grybhllqz.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqfvnosh.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gydidqzvi.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazejsjyr.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoxdizst.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/grapuxmjh.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/ghekwllfc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/grsrucihm.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gonnddvut.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkdyifaek.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gxkzhvfxy.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gagxmjysy.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaafxvde.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gtyinrhmf.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gidkmfack.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gajlvwfdi.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gomycroil.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gnqczybea.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvevnlau.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbdtfunh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklovpuft.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/glzwfqktt.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqctzwocg.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqyzzujlm.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkflhngmu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxpnjany.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gmbxyayuz.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/ghtjvlais.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gwhlwkuyv.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gbbszwypv.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwciekji.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyfvbxkr.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/greqzxszm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwdgrsyn.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ghmngxvhd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gxvspoyib.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gwdcxnmpj.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gnobknxlu.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjmxvenij.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/glcpooisz.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/ghspcqovy.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gkibcooco.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtmlencq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdizbrhdp.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gftasohhy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/giaedsabv.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/grxebcnny.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmokgzejw.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gfmhzenge.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxtnvmuj.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgianqoc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giaoakmmm.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqisyacn.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gohjqpskr.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbevrkynb.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmesnvgcw.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryjbrbss.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gyijbemus.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/ginmkxdfj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyckpdykz.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwzgjfqb.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrqyktna.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gspmreahw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gntgvsgbz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmudnvqq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gkfxzaird.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxmrrjmal.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwygfujzx.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gkflhnzbm.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyuckdej.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjsiozsm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjpcomtrw.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gbkexvacd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdepmxvsv.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/guoxvwzzy.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoczvcks.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gslxctppu.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gknhrbfws.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggxxjlpzg.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnklwtewo.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gkdvuxalt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkjvnyqt.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthxlwffa.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gvvjqrmtr.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbkvdokj.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gqejrjmkk.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gbzundqsv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsyyzwai.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gtvyxqiuq.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgluvjed.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyvndnmo.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/geoobfpzw.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gtcwnfjeu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbohxgns.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gfjorlsso.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gpcbveuqi.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/grqqajmji.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjzrdlnh.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrfornwa.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnxcwrfj.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/guzsorktl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gxrwizxaf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqduxfgh.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gdsndgnqu.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gymdqpkgl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqxoyetg.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gofpyotbj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqmscnll.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gpnpvhutw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gtkzvktgw.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/grbphaejv.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjswqvacd.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gaovoiesl.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/grabfbqqz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gawolrtwj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtiecvra.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/glbzxjdtx.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvgpkper.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbylbwjh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwbqwiuy.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/glifziyel.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqpbgpbh.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuahsvic.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/govhejyht.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmzhtwht.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoprygie.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gixauogyz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gqxumtwlu.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gqsqtnzph.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtozkkfma.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzghoocvw.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdexmcmav.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gfhxlummj.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/ghkxzorkz.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gnmumelzp.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gzdbowrlh.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndsyyvlk.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/grnpywxcf.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmpdddcz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcmtthrj.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gcovfsdmq.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gqlgedyje.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/govihsvec.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/ghluznfdm.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gecdzekbq.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/grepnddqf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkbuzwqo.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdxnrmvn.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwebrucc.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpskgnna.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/guktwsauv.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrzcnrwd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeneuhmo.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghegpnhdu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glrkqeubn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrqbdfie.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhbbgoye.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzpxcszi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfizzmick.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcdtypqq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvefddooe.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnroslcj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gscfoyztl.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gxmpkbcpr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgsqmjar.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzbytyccl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllikawei.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/galpmrbme.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gsfdqkohu.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqwtsfqq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gopwrwzog.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkpoucsx.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grudkntwh.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmzkqbit.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/galwjhtet.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gajirvlei.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjywuqsqe.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gzghswoie.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzjvlfocj.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gaeoggxmh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvngdsyf.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiqorehb.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gewalkten.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/glngohnvb.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcyvqgaf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhslpbum.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtzqwhok.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzlvxkip.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/glawccrme.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkeqjxgay.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/geqvgpjxx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gplbxxyhx.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgstzfmr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwqnidzr.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gngeguybw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlncycxx.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvfivocv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtqnpwtou.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gqcvytirv.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gfjegiaqd.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gubusvsta.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gkmpbhryo.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gojuyredr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/ghgiivftp.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyjeeayj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwfrtpyg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyntzecfe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gwmcitpxb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmyexeefs.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxefqcxcw.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gcwyysefy.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvarjilw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gcodmaxuw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctadatic.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvprdukdu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxamtgfzn.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqvsvihn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gesgujbel.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxzxvavq.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/grqlvtdug.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gldguugky.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcpmqqkh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gbhenuhda.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyvfmkwy.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gwncpppic.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwwfdskvp.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gixqepjul.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzdaszoi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gryxxehen.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrxltsxr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxwiyune.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gydwebeug.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqfwkzcg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqszklcs.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexmswvrj.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqvdkrsk.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gipceprtb.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gaogcmkym.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoxjfkrn.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaeeejgi.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxazsfary.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxaxvfxt.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiquwgev.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/girujrtij.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzeufeqm.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaemnrvd.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gfprukzwl.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gqplylmuh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gypocpfeh.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gusgpkydc.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gctbhibmc.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzhcnhib.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpmtobvt.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gizqhecze.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyujprrzj.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgsedtij.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkvlbwfo.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gunvuieyt.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gmjexsjmr.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/goobwsbqb.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gkzddroni.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gxmrxekhw.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhdgjqep.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gevhonlpl.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gizjlmphy.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gzamabygb.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuglwuqz.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbtuqdve.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gajzqhieb.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdufkmxf.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/guxnhmhdo.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gherqdsfx.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/giwfarqki.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gipxvfzno.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gtapkkvzz.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gjovfbsrp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmejxfxuf.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjoyndlb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gvofcxpue.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqejraqau.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gevmkqtqq.sHtML


<!-- 参考信息 -->