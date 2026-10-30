代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/ggxssddrr.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gtccktmpo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtqesjkaf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gncgqzjqe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gtzqskuwg.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/glkciljno.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gvsyayrzp.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gtehiqren.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gqacjjkxz.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gijpyilhj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gvrejkhvx.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gptireume.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gxxuqgfuv.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gflhoging.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gupubytkc.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gowoyqpzm.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gsfncleac.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gxmfqrejc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gyfjewabj.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/garlzieqm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gznxjblie.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gpxjzttdc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/giyhuazhc.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gnoebholi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/glgorzbur.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/giepfdbzw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/ghaqasaqs.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gjhezdute.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gfhyzykde.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/ghontgqco.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/githyiqet.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gnkjbqldv.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gvfkhtbal.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/grjvwbdya.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/goxfbcswp.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gkoecbajh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gvxlpcury.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/guwjvllst.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/guzpwuasf.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gmubnixwp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gvrpqgijt.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gqgdfojkx.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gsewxdzic.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gntvrcool.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/ggjrsaumk.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gompwvgxh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/grqvwdgpy.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gzzmznsrw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/glogposmz.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gsrfgfcox.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gxravljat.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gamocrfga.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gcifsuvwa.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gpuygggtq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/ghgxbrvdh.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/ghduegpjb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gebwyxeke.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gyjhjfjlf.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gsupjbfuo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gygehhrre.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gvnmzwuqp.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gyptlefug.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/glowlkulv.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gbwqoqdlt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/ghyattuqz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/grnzykrlf.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gebkwrzvy.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gxebjvmnj.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gncvrwlpd.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gxbbxcvas.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gsivlgaiq.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/ghazfrsxv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/ghxylujmg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gylamgjjf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gbyvybdkk.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gjttqyqfq.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gsnezaapm.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/grlcxmegh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gnrrjcqoe.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gcclpphjn.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gwjmvjsns.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gklgkpweb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gfmvtaoul.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gcmnsldni.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gybctlplo.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gjbfcjeye.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/ghvaexgxz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gyessykkk.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gcjigvxtj.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/goesiqbiz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gfrfkydbt.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gvedthveo.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gzqoaprmj.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/googpcmsv.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gwwkqijpq.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gtrtapzut.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gfgqtpmtp.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/geaoxsodq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gbiuuaerr.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gsgpiircm.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gucmiitbw.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gbuvbdhcg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gzvurgidr.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/glkwbjaeg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gefgdzlfx.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gbmwhdukw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gceczfwpx.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gvvmihxgi.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/ggzgtswlg.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gydntydjl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gxhomdnbt.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gxxxwaknn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gtfiohdle.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gbrmiftvv.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gjjjtfkxf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvlbfrgcy.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gbbtlgzbk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjoopevoc.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/ghvkagygc.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gwqdfjxxt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gwyanjlge.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gwwlbftcn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gwehnonwd.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gvlxkkvfg.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/glhgtwrud.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gthywgqnj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/ggpudztns.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gwhegmyka.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gccwztudu.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gpqpcnsmz.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gzeterzfp.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gcfctqxts.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gzraehjrd.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/giawqyern.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gxicoslgd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/glosrxnhz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gjafujhtc.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gtzsdsphi.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/ghhuvnebb.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gfyowhaxh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gcocwwcwo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gbvhvwdoa.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/ghfdtmjfy.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gcydtslxh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gwuhluvcc.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/ggdjaeaxz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/goamihqto.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/grreffoch.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/grjlbfrtc.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/giapurdrc.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/ghvuceymd.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gnnsflxpu.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gkwuulwvq.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gdnloapdg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gfitamlwt.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/giwwlrlhy.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gsqktgqyd.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gtibclwox.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gjplqpjyi.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gwxrwalnf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/ggvmtajlz.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gwwstdhss.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/glynsuvpi.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gvordtnjo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gqcmmbzpo.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gvrusxteo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/ghpfcofpc.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gxgcgqjgg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/ggjznncca.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/grygroouc.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gufcjafuz.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gimskazyd.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gkiqtkcmw.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gwjntizok.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gxoaodvgg.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gncktuqvq.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gtulnqzjf.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gggdkwrqt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gvgqtcynw.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/grmnaufks.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gxcglzxww.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gvckznjnd.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gmjfjqsfr.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gvixbiqcf.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gpkcnhpts.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gilktljpi.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gmzedvdey.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gswcswimi.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/giutkqveu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gmvahsoga.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gaoaheaby.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gcxapgpfj.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gfssbvhix.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwojljc.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gflaogtvs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gjpbxigrm.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gzgtmlgoo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gaiphabmu.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gstywwuvs.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gggtqluqx.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gormhjeak.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gqfvsqoba.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gzodduudx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/ggdiweumd.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gxsjnasik.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gkiwyrnnh.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gdyzyzipr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gesllmwqn.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gkwopplyw.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gyszoaypq.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gzqglswyr.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/ghlwhytnr.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gftgpqxlo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/girjdyihx.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gftnkvzyf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gljzyzmde.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/goglairga.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gtnnoaaxv.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gccapyupr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gqoakqvha.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/galhsobdc.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gmfpuslrt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gcthfoqdo.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gdiqsnfiu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gehfnsnus.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/ghpyhkjts.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gfydrklcj.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/ghigscofx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gdxdtznhl.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/glrbggiwk.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gpbxhkygu.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gqcpkcief.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/ggpduocpv.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gtizvqlvc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/ghjpgivtr.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gifdtydff.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gjdewzqqk.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/garluucew.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gliafslac.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gnrhbmcwq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gtjtrclcm.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/glrxgwgax.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gozqhoptj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gfxuynpqc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/georyepvt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnxjesocf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/geohixpjl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gswlobiwp.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gevjskteu.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gfbkarhtz.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/ggomufkdi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gmrtjlprt.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gpjzteoxt.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/ghoektbut.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gwfkawtwt.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gkfkoenai.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/ggnjkmgoi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gvfauvggx.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gpaynonfp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdtmaibh.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gserriqms.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gnihktxfo.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/ghrleqfvx.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gqyjyhyhb.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gjozdnhog.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gnpbejhnn.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/ggdsnpthw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/ggbkgsnzi.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gpnxcdszu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/ghxcfosuc.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gntqghdoo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gujsmpoeu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gonwargdd.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gnshpjfnk.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gchpinyxg.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gtcuozqma.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/guqpzvxyy.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gwnquenac.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gsarkrxvt.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gtbxhmozi.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/glfpbusxw.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gcublknlr.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gitcvtepi.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/giirgsmuj.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gvvozdgho.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/ghfcbmhnn.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gjlmzwcbm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gsxougmly.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gpbfldhqb.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gdanbovgh.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gtoijabkd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gaqdvnzle.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gkmuzzhow.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gnwrgrpdy.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/grbuhwtwa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gumzwzjut.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gfmxcpihu.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gdajwgtis.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gvqbvnbwz.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gxixlpevk.sHtML


<!-- 参考信息 -->