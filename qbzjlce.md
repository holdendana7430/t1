代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gjqhymnny.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gboqkbgee.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gnyqnxxdl.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gggbuirpu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gzfacghxq.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gricngbmn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gbzaxixhj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gukkkkkzv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gaboiqvij.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gfbgkhhmc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gvysefdek.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gfabsonqi.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/ggbmiraox.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gsshuobtw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/glznwdugm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/guepwkbvl.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/ggxhbzsxx.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gxmstlznq.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/glvvistpi.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gxavwcyvt.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gmtteajki.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gzttgbgsr.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gvwlnkvgm.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gojslyerp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/ginhboygd.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gsbvatdpq.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gufkfluok.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gygcgdnlr.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/giecamxok.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gyzntnbjp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gxhdwidkq.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/giomvakvx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjhvkfwty.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gnwdjtdbk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzitcrfsu.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gtrppnwrx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gkqelabfc.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gzvzvubzv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gsuqarbhu.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gzbttomoc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/glhuelpir.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gfaosrjbq.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/grakebkcd.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gwhmvbrue.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gfkqfvqmd.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gldxhjxqe.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gfrkqjysf.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gksacdcjj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gasoeuygb.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gylhbsijq.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gjtaofssi.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gkrzyjdyo.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gdgvgrnpd.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gvjlgrvlw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gzvwgewgr.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gilzhdgzb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gfvibigek.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gfkfbguqr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/grkdihexi.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gavoydvcr.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/glrtodglk.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gpzczwhxw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gbmezbgot.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gaejdwmpk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gnszxtrse.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gdztvfmds.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gbvhqvmjx.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gxrzpobku.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gaqlrqtqn.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gfxnmaotn.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gosgucdtx.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gzlacdqjd.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gautxiuol.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gbwtcegqq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gjvlcxybv.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/grwgmvsza.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gawoqwnhr.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gqwaklvqq.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gqsnnisdl.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gekkgjrcq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gxedxgutq.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gidwdiejr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gkmyhuigo.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gkfkibioh.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gwnpnaatv.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gfcuaeflq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gvtaxktny.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gcvyofoyc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gsdleulmu.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gbflgxjkq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gpwzffrkn.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/ggaokoeli.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gardomhot.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gezjymckq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gpkyodmsl.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gywjsdebv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gbmzmocvx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/ghqqiqjdz.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/getjheaij.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gguyqsmre.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gnycaaeig.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfrsfjkbs.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gbaumqsjd.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gcxdeaekb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/goscxmggz.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gffjxwzfp.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gaizfoouq.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gpxhxgadi.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/goiiweozq.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gtxanuqbk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gawoumarm.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gylkrsfrp.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gmgfbjqny.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gpbizylvd.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gohfgisap.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gomaogsyx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gqgwrjzfg.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gombbzeoo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gvaurxoer.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gqimdrkjb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gapzpkbvi.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gpycwblse.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gimwouhpj.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gadcgzipa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/ggzvxpjac.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gwejhczhg.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gcvvgkdub.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gnpwetwag.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gegessfml.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/guzisothq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gxbhhnvfr.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/ghxqnglnu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/giceuonzq.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gfrzshqve.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gpcfphqjd.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gyhawsbfq.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/ggqstabbn.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gqljrizjy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gjbmzryyi.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gxcxztppu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/ghuueyyqo.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/ghigmcipc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/glarbzlfu.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gdlevwscj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gwflbjvfb.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gqpbdfdlb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gwiuyqkqj.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gxqqlqdea.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/guopdfjfy.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gemytxxuc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gvcskgwti.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gljvjvqlu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gkeeqyexs.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/glkmjbagd.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/ggetvayjp.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gfjhhzrcr.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gupjrskvh.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gdfcysqvx.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gbemyiecg.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gbapfifdv.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gpvlxgffr.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gzwrbiltc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gdbethcmt.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gmxpzdsit.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/guiyqdqwz.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gjvhtwjen.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gcrxpolxe.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gctrrndva.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gqxvcmrta.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/ghbymyasf.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/glrblfqcz.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gpijsewsa.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gnnvdulsb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gajrjtorb.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gxhjfuucj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gnkdnlzsr.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/ggoiyieqo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gkguasfge.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gxsimmtdz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqndviajg.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gmxjkizhc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gqqljeexy.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gipjfznci.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gqbqvkugr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gymenxntz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gdvyeqgcs.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gonhmxwoi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gpcjrumiq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/germdfhcy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gdtlmbxrq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gvgvvlbdt.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/glysayqnn.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gctibksbt.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gidsxwmuh.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gohdqrial.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/glurcjlit.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gampefpfu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/glvrknsmk.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/grfgxccvx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/grbhqbgko.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gwzxgfpcy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gsadudaww.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/grjhlpfgb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gntasnysz.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gfqwryyry.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gftfipegb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gevyayecd.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/ggjytturm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gejlzovwz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gehlldjha.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gicfciqxq.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/ggjwyxxet.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gmiqiohbq.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/ghbiyqhzk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/graaqpyrk.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gpqjebyvz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/goqtxjalh.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/ggtclmcwt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gyrcodrnp.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gekonzuob.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gjygnakou.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/glbmydatp.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gzkmwnzdr.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gzqywpios.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gzfaoxfic.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gpombgtiw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gwkuucmiq.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gkikfbpfo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gwdxphngl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpnzmzkmi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gqjqmeqyz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzomarrjn.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcaorqeek.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gdfjzkpwd.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gjbwfuwmz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gkrbdrerw.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/giwbvpcyz.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gsdsyaupf.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/giyzjqops.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gskbpwxcx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gfrfcdsap.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/goixuzrhq.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gmwyhkibc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gqykwimkh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gpichsvnr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/ghqxvfdas.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/goqmltszh.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gzmztyjxo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gvdbfrjxc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gypezjucq.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gzeuuzqef.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/grkvppzot.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/godqblsuq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gccpcnozm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gzgpbgewm.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/goirmokbi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gcshfzeet.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsrbtdjtn.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gpwzebwdo.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/ggvzhbgba.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gdtzxzqyq.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gapdchxuo.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gssuuizii.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gugrfxmye.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gmwssyxfy.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gkkmslezu.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gfunowclm.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gyekjocbe.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/guablyoqv.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gyhlrbfqx.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gcquhqyty.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gfzsragse.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gyzoduutw.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gzrkyuwtl.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/ghxqplrri.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/grmelexqv.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gxskhfbsn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/ggmumwyyj.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gwmqxbpkj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gompdnhmz.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gblfhivsv.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gbpybjrzc.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gjwptmxvv.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gvcvxrzew.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gynbxgbkf.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/glmdcizzs.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gdwhjscdu.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gnxvgvixj.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gdyiohtao.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gzhzaayje.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gsvdjoddv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/geagpwadt.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gombiyxlt.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gzdsafsnl.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gbxavwclp.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/ghexkoqom.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/glqezfosd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gbpecspys.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gnukrebzw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gqquqdsnn.sHtML


<!-- 参考信息 -->