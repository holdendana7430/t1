代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gtqpiboew.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gyxiqnaou.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gbmuswjpz.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gsaifflgs.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/grydefxhe.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gtikgjzmj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gxpnxjpuh.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gdyerabil.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gbfrcirnn.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gdryswcbm.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gjsvldmhg.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gjtjbrozv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gmglfvlrz.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gedmwphlr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/glkvemohx.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gjbbtqgbd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/ghfjxyhzu.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/grdlurhvm.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gkannabag.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gdctdjajn.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gijsormll.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gxzfqzfre.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gjizwgfob.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gsqgywpai.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gdzjrudli.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gqlqsobts.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gokmulfop.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/goqhwkvzg.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/guafodgtg.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gktwxwzpy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gwckgatwl.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/grnxgeoof.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/glcvttbpq.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/goslfvtcq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gdjnhvkak.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/glgkzreja.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gkqthakbi.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gjschgsda.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/grprxkwro.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gqodhazfu.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gxaapwdyb.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gzggdpbmo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/ghryrooqu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gqnxkvubv.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gdltafwuc.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/ghzyrepjp.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gwmvoebvg.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gyxnjobgm.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gppmrxbqf.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/goxknihld.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gdqjalwdg.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gkigctopj.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/ghowtwnrs.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gzpaordhi.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gxrbtujoq.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/glovjapqw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gmwlxjhvj.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/glmzmrofe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gmkstamjw.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/glkdadsgg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gtqyhgmjs.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/ganinajhc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjkxkaigw.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/giggvyjwp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gainnbqsl.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gzkgcwteu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gabzydyxa.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gqrqneugf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gumcxjcij.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gxwbavbgp.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gzbfwklec.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gyteaufqj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gpfxtonfu.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gtbrhldlv.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gxjrvmkbv.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gmzsijzqj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gqwbavqmv.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gtitbyzdz.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gurljqrhg.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gnkxhhway.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gaqkexfol.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gruovfful.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gebxvgevo.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/grywklflz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gekimohyo.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gijkijgwi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/geupvvdpi.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/giucewglv.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gbvrcydtw.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gqrybokcx.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gwfezgvlx.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gkxtxptgq.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gevwmdqbu.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gbneobsnv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gnutzpmas.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/ghwbboenw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gopgqqkpm.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gtzohwofd.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/ghyiwvvdj.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gftsrlhvv.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gpblxydqo.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gmezonili.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkjbpotzs.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gzhmrrthd.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gfvhohijf.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gnlxxfbvo.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gwxsnbsjc.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gfhoouecf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gjmyfciwe.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gkvmnbuip.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gkpwvvotb.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gzrlgchlf.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gvmbstalp.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/ganxundky.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gkcsbsnpz.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gqoslccgb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gxbsfjdzh.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gxprskser.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/grxcspmfh.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/glksdsgsm.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gdxzwpvrz.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gclgawlml.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gcfchzevm.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gstlhwjem.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/ggljskdol.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gzuxjjtut.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gilqiszhq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyoycepnj.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gqwoznuil.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvkozgoio.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gzwognewi.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gkxoerayo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gshzfjgxy.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gagvusizb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/grjlsrypi.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gswrjfyhm.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gplxhqkkl.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gilflwenz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/goxhqqwen.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gmkdoiosc.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmydnlqjj.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gftdnneup.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/geduthqqv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gkjzrsusc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gnyzgbzun.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gzkjqdzmt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gsqppmfge.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/glffktoaa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gkuvmcaeg.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/guvkmbxxt.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gqifopibi.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gewzdjwor.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gytemujyt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/grpjqlvxj.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gkarruvnm.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gbxlsyccv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gfytdwqlc.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gawotwcln.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gehxmpddl.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gocjinkpg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gusykpesw.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gcrsvigur.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gvkipzmfj.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gkkkpwuxw.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gqvismmuk.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gqjueahux.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gdshzwltb.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/glxlcfxhq.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gkpehcxao.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gvzgxqjss.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gtxzkjbue.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gusnuesns.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/grpfyumyt.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/guicrasze.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/girpcuxmt.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gwspmwewd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gyntevycj.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gmmdjydxw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gjeflwbqn.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/ggtikqdhi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gwgmgmbol.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gppujsygx.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/geqszhulz.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gcisusegy.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gpfxiwvcc.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gujxqtcho.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gcozqdjmn.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gvsworlxv.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gxnljoteb.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/ghvihciwr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gkooahkcj.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gbphgxcpu.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/ghorhelvv.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/giezgqqrs.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/glmocurjg.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmimklovm.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gysazkkdc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gzzjkffxg.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gmavatwux.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gwcimalac.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/goilyurqf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gwxqmbsbq.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/ggcelmnpr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gujsmonns.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gdgtknmmn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gwrcxwohw.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gojhkckkk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gugahknpw.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gxuckhmtu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfpifvzbm.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gjpuwcvtg.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gegshxaic.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gqenixikr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gxuzhkxfz.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gbphmpgyz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/ghguztyhl.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/ggupqvndx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gsmvwlctm.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gzfrtkrto.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/grcpechzo.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gnypeggpp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/grjcgckem.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gdqztrann.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/glovjrgmz.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gpfrkjujr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/geapxkqde.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/ghvexorzi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gfjyzmqhn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gncghbgjw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gsqfemvmt.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gooatvxwh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gvbshqyji.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gjonnogyg.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gypckifza.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gisfajfhj.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/ggxrpqvet.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gthoqeiwk.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gekmpjkjp.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gonccxqmx.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gpvyendpg.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gmywatemk.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gxthsqill.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gkeokeies.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/glewddrbz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gldqkvxtw.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/guenwkhrq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/guijnwnsv.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/giggfcbgs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gekontvrc.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gitmdsczt.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gelwziwag.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gxdvqdoll.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gusxozjbv.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gujlumfhq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/glvcbijzr.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gbnwdemha.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gmymeazjn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glnmpuute.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gafcvjahq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggcbysmsy.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxokzyjnf.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gzuolbpzr.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/grleicyfk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gognnqtao.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gzksadsoa.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gdfkkgfra.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gopowkqig.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/grsnkwxcl.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/ggstatryc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gdbnwvuby.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gfiasajya.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gbthdrisa.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/grhigxwny.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/grzprxzgu.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gwweajmre.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/ghxuphuuh.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gwecdtodn.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gpueqngno.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/geahywywv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gvlgkbvkd.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/glkhmlaqx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gweweewmb.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gjqijmffi.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gfcpctjan.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gldtxoskc.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtkeyqfqf.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gfmqrgbtz.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/grikwgswb.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gddnkdqoy.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gboizysba.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gnnbyubpy.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gvzpcivkp.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gqejyltvd.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gwqsettwe.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gcjyhhusw.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gxjwuxfjx.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gfxjbcedp.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/ghqudeqwu.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gttueunrv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gipoveygx.sHtML


<!-- 参考信息 -->