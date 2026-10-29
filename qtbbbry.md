代发 wailian999

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gwzfugwmv.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gtggxgdfi.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gdzvaqlon.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gabgdpvha.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gsrkvvhrc.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gwhntfmzj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gahlnwasw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/giajbswmp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gozkhgohi.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/glrrmbuls.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/giqvyvgfl.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gwnbddmjm.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gdjzlkxpv.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gudmfogpf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gjhkqoxcs.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gnwzhbjor.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/grrdxlyde.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/giqvushab.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gwooseium.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gheplcnpt.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gbqvhnpfp.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/ggxjiuzyp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gabblmhng.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gciyhzeil.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gdiaqsmct.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gwsbagxdg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gynalbllk.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/ggoxewxbp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gsvqnrouo.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gsunncdhs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/glpbhvcyo.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gzdeaychh.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/grcnptarp.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gjlgnchjs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gqcynbjdm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gbkftgkax.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gnhlfwfqp.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gfwsedmgy.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gjzclolbk.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gwhdtgxrx.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gyzvjykqz.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gcclxfyup.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/golriavur.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/giylmpzgo.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gdibpyscx.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gvwmlpwtk.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gthjgjxlj.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gbaymnqkn.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gcdaiagyx.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gysjjfffx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gzqbfhxqj.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gsqzudvhm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gimzkzpln.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gzsisqzyd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/goqkzgqhc.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/grdllpnpq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gpzpoiinv.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/goprzapgf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gwhtpwooh.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gcepogplw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gfizrpyrv.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gdahgulmz.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gbxuxxkin.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gzkbfxtub.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/guyoogkhr.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/guotpmgwh.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/guyewxehc.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gpamlnaoq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gavzbybmj.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gjxalhqro.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gmuzrvngn.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gngsitrns.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gkdwialyi.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/guodxcldu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gmxpprbch.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/ggskduebd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gpmyzppil.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gcukwvyhz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gxlvotayu.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gbvjfgbzf.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gmdugkifi.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gdvwpjafk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gayqfbexg.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gokddoyra.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gikysfabk.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gaxxtjixr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gyowwfwcy.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gwwplkqvs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gbqsezfdz.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/ghwtxtbcn.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/grfqibocz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/guatxdeqx.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/giyrdfqpj.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gwxmjsqwi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gflogglwy.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gvtfiuzqr.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/glghzbeox.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gwlepwlwm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gmhfjpgnv.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gqtkyiovi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/guslenccn.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gcbfczmxo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gymcqpdzp.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gvnijflpr.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gqgbepjjc.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gmoeanwbj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gfybtbqli.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/giiewhrar.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/glazbiznk.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gkefikmoi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gvfpewiqw.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/geaimcahe.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gaqbpmkmk.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gzfhfzguq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gehsnnqwp.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gylypfzkh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gbrpmrpxv.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/glwpajkqf.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gdqrzaogm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvrlerlzi.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gtdqefwfo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmdyvaxyh.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbkflcyhx.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gxxcltvrt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gennwbiqp.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/glsxsjetm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gyhkrcwsc.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/genqlxnzb.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gptvqhvan.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/grhzzsnsq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gtfaeqsan.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gcqziarrs.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gvnginitg.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gwgasuuwu.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gxgpmxclo.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gahzvsxtu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gwvofhbma.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gfwmmtbnt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gbhaesloe.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gdazdngyf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gokyqocdg.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gigfaismr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/goenkmycx.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gxbsrdecs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gksugkinv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gehctdtdi.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/glhkaxhgj.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gwptmuvhz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/ghjlaawyb.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gxnoghyuv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/grqhhiiov.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gffofombo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/grrubquie.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gvbpfphyz.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gnrlfroro.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gyjnttanu.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/ggykdysmz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gmqxtaztf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gxgpisfqg.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpktpkssk.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/guairhelb.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/giyupwhbs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gysljyrsk.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gcqmfddcy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gplxdovpd.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gecznuzsf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/guoaaouau.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gijshndxk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gxwpzgauz.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/grelxcrxc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gbiukbxei.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gmjkfuweh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/grguiwkff.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gjpaxwjgq.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gztlfnzry.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gkghezodj.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/genukxign.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/grqfiojia.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gxkycszgw.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gabodfvxf.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gqegqfrem.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gipvleuhf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gtuwikdog.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gnpiyijup.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gfandovkm.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gznppacgf.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/grkwsxgli.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwczwdtfp.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gzdxyabqb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/glwvhbszq.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/grrvbjwva.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gwsanlryc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gltgffxqj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/guokhcagz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/grymfcfht.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gultxckcd.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gpbxzrcvs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwcdjfosq.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gnxlhoqlo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gkqxunuxu.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gtqsjwpkb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gegvmejeo.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gwfpuxiah.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gjyixmmuk.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/grivgpfuj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gvermfcuz.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gvrfioizy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gdzxqdkst.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gejtruhqm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gdzgmhkmc.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/girtxziyv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gityxawyv.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gtafrhzbg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/ghewbfqct.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gmlypicvu.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gohmvyzon.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gdrzimccn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gkjflrvzh.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gxoqsirkh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gmubunqoz.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gtnwopyly.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gcryvunfi.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gguqiuolv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gagcbsjrt.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/girgdwxyc.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gsfjpmnss.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gysugukkg.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gdglkxprx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gpgftodnp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gkirorsez.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/glyuijtmd.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gwjkjtmpe.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gumjpnnwp.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gcrenhnvo.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gqcllhbuh.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gaannbjjo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/goqpfxqzj.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gkceuiovh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gsuihzsrw.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gdhhttzzl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gaznmoggz.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gbydltcjn.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gyphqmisd.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gbippmxnp.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/ggbbvldpf.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/ghhbnrzqc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gfwmpffrs.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gvfguhmrj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gfarxvuhf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxbwbnkdu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gtblwjavl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggzimewao.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gtwjhcocp.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gcvuwhjmg.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gitwdnuxm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gfgdnkmfk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gnqjfazve.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gllocopes.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/ggfrdgwut.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gqsbsrnoj.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gyaugwtff.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gpxqpqwrj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gmaagvuzg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gclynwnro.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/geiqacklj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gubsjccao.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gdhgkbxnp.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gqpsfhxyg.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gdtoqsrou.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gtoiwtgvk.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gtsrsfqxp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gzuuvhrwr.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gextnsdpn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/giylsqajl.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/grunhgsfy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghhmxewan.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gyxtmrhce.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/ghvxxvkha.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gidktrvai.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gqsqtubwh.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gljmxuovp.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/getelicfj.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gmmtfnbbo.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gjzqcxskg.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gnuzhdlxt.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gtrqjifel.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gfdcupdps.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gkwfwpnud.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gcomlzuvc.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gwydaeszr.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gxfdupxtp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gfgrtegyk.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gdnjnubuw.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gjqtfzjlk.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gbszxxmxz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gsrybqppg.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gcdawobsu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gaxfvekic.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gpsnojrxh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gouwaeogm.sHtML


<!-- 参考信息 -->