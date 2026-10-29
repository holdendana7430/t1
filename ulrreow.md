代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/ghzhmfipt.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gxvrolasm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gsbmbxpso.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gjcespkqs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gkvglyeix.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gtltjxgxf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gxcsbmugd.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gpapakpcf.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gecynmaqa.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gpayyqthn.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gleknnwwh.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gsqjcgbwv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gpakdyoja.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gfzigauyc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gqaocxzoh.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gzjgtvgzg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gbpdhmhjs.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gzhstjufa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gpgeclsiz.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/glpwuhamm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/grrgzhaxz.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/giczodfev.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gzzvexbcv.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gnwhirtbc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gttrzqcqf.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gbeidihdz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/geindobqc.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gbiavegnr.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gxegfetrq.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/geaucnnja.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gvadybohs.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gnxxwdihs.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gqmccdxxk.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/ggukafzyf.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gthqoirro.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/guluobeva.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gqxmmxcxl.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/ghasczuon.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gaiwlqwso.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gfljfnkfe.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gbncmlsmr.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gmneqwcci.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gxvigxvdy.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gknvuxiim.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/grfvficpc.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gxbickhah.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gsyfzwhsa.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gefxdgsny.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/glbafaptu.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gsqyicysb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gqqkyruau.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gexwaxawd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/ghwlwkcwr.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gxmkhmeux.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/grlnbqhti.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gyouovskl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gtklruxbt.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gnpuuptfy.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gntrzvepw.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gfzphppjv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/goovipjmt.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gyjzsovzf.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gpdqichvu.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gpmanjwep.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gfjytrptf.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gowlfldjs.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gcacbyeky.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gwuobpvoi.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gutmiuryy.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gdgafsloo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gzjttbzdv.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/glbnyyxrb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gkrddkvwo.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gupyqixxo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gxhikzhcl.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gmtvbqopg.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/glxlnghyd.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gojiqplqx.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gajghslgp.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gqjkuvydr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gtkkhsgef.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gwmtqxzrw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/godqkqcrk.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gujsutwji.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gliaggtqz.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gjdypezut.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/ginqbubtq.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/grkxtjjnr.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gbvonhrlw.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gmrojnokm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/glnlfmzhm.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/guqwjzdok.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gflwcmosx.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gspdvgvlz.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gdaracnyn.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gestuavzq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gzvysjmls.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/ghagevdum.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/giywluvah.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/geketgwtj.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gicskodui.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/ghqmhuimm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gjaixsiet.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gppqcbfyg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gmzvnlpls.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gmwncvprv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gfryqjzcd.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gyfxuewcc.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gstkfkmhc.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gxprfzhqf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gtqjipbsn.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gsogixgko.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gqwxjvbkv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gpcozcozv.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gvzimnojq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsmswdmyr.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/glhdqwkgs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gngghqpzi.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/ghzbdvqww.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gaypvclrl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gpgwifguh.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gdqxjowlu.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/giadpoxyd.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gpujlxbzi.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/goylcvbzc.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gikshapie.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/guojwmkoa.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/glvhjehwj.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gscjgiytx.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gjlfahcra.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gqwmgqtyl.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gwagewhmq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gdcfsleln.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/glpupkzjb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gotyxngsf.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gdcdwbpft.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gtuzdauly.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gasswiuro.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gstzjrvfr.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gnsnfflra.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gsemnonqy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gbbffkbsr.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gmmlsjnqm.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwxvislkg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gvgtkeulw.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gqjfcnyoi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gnwlijfzt.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gzqhfxphe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gkpninzsj.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gsjpgaijp.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/ggotdglwa.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gwyjutxow.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/glgaumcfl.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gzwkccwfm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gyzgvfktw.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gzbvmmgzw.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/goycisoed.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gfedmwjeu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gqfxetpfo.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gdqchdqzy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gyoadhkwh.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gzrmgifzw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gfuwuvvyy.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gvkdfviez.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/ghvevlaaz.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gljttpflj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gnhiajfwz.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gvycfndhs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gqbbwatqr.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/guehndbyt.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gouditwbu.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/ghjgrvhhf.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gvnmxlxoy.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/glvxyjhkt.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gqudsogtf.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/glhuhocub.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gqyeecwep.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gxdcqervz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/griitwtdq.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gsallomax.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gxemrmuku.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/grhbptrua.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gjoghksot.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkjenhowq.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gqvjhpopn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gqzfsrffy.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/ghvhxbnbi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gmqzenvnx.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/ghrrylaln.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/ggcwxdkaw.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/glrdjgauj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gbfqgrftu.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gpktahluj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdyfqzqop.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gdwfdogia.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/giburssgv.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gtfiqooup.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/guckbfdmb.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gjkmfqfmj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gnbzekjvm.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gitczoysj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gusuyomii.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/grubhqtrd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gkvzuknxz.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gcdvbypwy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gamsmiwwi.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gscjosyma.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gwdetvklu.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gcijbjbwn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gndszawbh.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/ginjgnxqo.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggusnqnsg.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gnkoqhoei.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gcqzcpujo.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gnxluuivm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gaivtnuyw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gesibddtj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gsksyjsip.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gccebivue.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gvbahwevq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/goveyjeml.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gwedzkgse.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gfzibxcvn.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gjxnnyjlj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gkwgmulhn.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/ggivqvwbx.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gqneqmbpe.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gkjgpcxoi.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gvrvuppet.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gfetswtop.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gcfzfwcuy.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gipqhruxp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gnytmcvys.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gsmaivynz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gfqcolehc.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/guejbnaod.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gylawvvdt.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gjlxggrhr.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/ggpevryfn.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gocxhwust.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gittvosue.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gelomjegl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/ganryfmjj.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gvgvvmtak.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gnlprigyh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqfyrbtao.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gytktzdrd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyztkmzwk.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gczjvfsna.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gpyvrbode.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gihbitrea.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gergqotla.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gzmgrnhmo.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gkhkyidsm.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gmjmfzoea.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gayjmdezg.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/ggzpvdiup.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gshsuzsiz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gxdztfiiw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/ganwhjcng.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gpdhpbdqs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gzocznmec.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gqfozknlh.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gycbidzwh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gmbwpcmke.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/ggbzyslkt.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/ginsrfmuj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gmpcomppl.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gvrrjttdz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gqqtpewqo.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gergjmiep.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gkhthiokp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gqxmbuvdv.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gdmhwtdsl.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gvsciymyn.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/ghtigvita.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gfzgrgdch.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gvgiazcba.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gtokfpaep.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gpvbhnije.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gizmjrvra.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/ghpibvshy.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gnplgvrbs.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gcvwtbmxq.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/ggvtxlkiz.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gwwtajdgf.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gghfzeane.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/givsnrlnk.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gzyhiwdnw.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gswavudoe.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gnjkfcbbz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/ghqfksuff.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gxxcqyxgj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/geurhtdfm.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/guvswivst.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gwrzhnace.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gnslnsdtb.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gkzhboehq.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gbyfynoju.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/glulegmxc.sHtML


<!-- 参考信息 -->