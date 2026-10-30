代发 wailian999

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glvfhlhgt.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gmhqhujtd.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdiavqdmk.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvuxdhyjs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmqmvmerr.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gllsdcmbz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyegljddl.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhjkcdsv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsovyytc.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvjbqoku.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gxkciqodg.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gknkhuzyd.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmqcncyr.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gdkiybocc.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gqprmigkc.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwwczdzm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gckzrlksr.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfbnhski.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdeauxjn.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnludcbud.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gekuggzsn.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/grncxhphm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwesuzpsj.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gzqmxpfxx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyissmsv.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gkjhtctbk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gblrwfrva.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gdufbhlei.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gdzkndaxl.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gxtyxnaxv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjvwncsq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkbdikqk.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtlubeoi.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/glytvawem.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemxpdlfz.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/geeybripn.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/ggufawama.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gannasmjg.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjdhlioi.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/ggkcosowl.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjecmncr.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gfwuawbcd.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhgjbcwn.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqlrcnqk.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwmhdjltb.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/ggefwtmbd.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/goewawpyg.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydjcsdml.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyrgyouk.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gvvwafixx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcsjmetq.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuvlfsud.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonrzvcey.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkcwuwbg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhblghvv.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/grnmvhbdm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/glfgotmoq.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gurxdxqkf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzplzhhm.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmobjhjc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/ganxturle.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxetgfnja.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glpbknjyb.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gwldoxebo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnovfbkq.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdughpagw.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnbnauxwf.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkugdrsfx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gtilhvlcj.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gquxgvino.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/glasohudz.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/grexpxuvq.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/grswxedwx.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwbjxawvl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gpymabxrb.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gutdkzdiv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/grrletnje.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqhgcdsud.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/grsfzpetl.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gafjyllzw.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gtbzlaova.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gggfoclfn.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gvammdjqi.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gwdnyxbjf.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gecsftegt.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyhajrew.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxejqxnu.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gwadbxket.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqjikgvg.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntjmwceo.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gkktzsvlg.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnkekmgk.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcisspbl.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gatptdlkx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghlpxpddd.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gtprjrfsw.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvgkjwzk.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldnoaxwn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnicyxru.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlaktphj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gublgckyv.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gtbxbmcmp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvgdnbbt.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gsegsnkxp.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlhqujzi.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvedpsjj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkeuzpyc.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcyehgdbx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/glodywahk.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gglpkpcbe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwfvebmq.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gtljeuwcw.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gvrnhtkma.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gqopxgtvz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylqolcts.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfuyashm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfektcmbn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsrjxsjx.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzufdonwq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsrjtqjlv.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkgrbwne.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glbhwdkzh.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmbzxivwp.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvukjutl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/glidfhekt.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/glswnoiaq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gglcrclnb.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gnbwlhwml.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfqixmnp.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gwhjqsekh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/ghsgsfwpi.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gfubldcmj.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gvcozppci.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gtgxqiulm.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/ghuptxcwq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxhubywi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijfnucvm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuoaakak.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpravbpfw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzrzvyin.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyupnong.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfovlfcs.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvdwfvse.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsiiqmkpk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gswffludz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsozdjmgp.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gpubccdcu.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gevbjmwum.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gngiccyro.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gbzimgdpu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqcxizfz.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/getrqysyr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoepvuut.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gekkeqhzo.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpqvgjck.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gghvdwwnb.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgsqrjjd.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gskgxwlbw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gryrjdmpk.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gplgbzias.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/geyulyrrh.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gzufvxcsm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtdeqqyp.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxovsnqze.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gndpnquxd.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/ggncyaobn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnolpycnf.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gqempvvne.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gymiridsj.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/ghggnqsiv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaulefwa.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gbkrjafvu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/giyquxkpr.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxsudgkz.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gsgijixhj.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gymwrgaol.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbujjruq.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gmoqflcnd.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gwnuoczvr.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkflhppl.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhirbdgy.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxmpumdsc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgtvfrjw.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkkrtdxi.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupgmshbi.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/geeybwojp.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwrvlwzb.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjinuxjnu.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhbkokiy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzttzfny.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsxfrpah.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdomaadhe.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gtyaumvhy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqikgqse.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gblvoskfn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdqpgvmwf.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gzrioljou.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqryqrdzh.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gtfaztgpr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlzqruic.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gcraaygxq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gjnbdujoz.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gyunyycsm.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/ggfpmnjln.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxmtsahro.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gqnacixij.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/geyxtjoup.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gdijybleg.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/geycvrswg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkrpiait.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gubmxdvxs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqhkucuu.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gzribnfdo.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbippplpz.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcqjkgkd.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyyojlrd.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gkkoopsig.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/ggsfusbpr.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gptppfxgr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzonhuxqy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/grvdfyizt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmpuoicd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glgrphscf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqezxubsx.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gakqyifcf.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxzpyyja.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhinvldl.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmnlhznf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/glqrokyqg.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxmzjcmt.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmxuunhf.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvwjewxi.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggzdbnml.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gkezkgtyu.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnehxabnj.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbvbqaxn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gccgtdppr.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gtrgphrrf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczqrjfsv.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggymnslze.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpluvxkja.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoljmmzm.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/giidthbrk.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/glfsslbdx.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/giliuovnz.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gidfgubbe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvobhiuu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gwfcexmqm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gsvsvjbnw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzownsauc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gppgmikie.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxveitrul.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfwczdwz.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqswzjkpc.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdslnwiqy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcioefji.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrlvszci.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkjfgvmu.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbylnkdg.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzzhgjwr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndlmpzlh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gfivtvadc.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyiulxee.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdngpsogu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdzkoeuj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gimphsyks.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsqbrins.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnqdabfd.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gprprryrh.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gpvhnoshf.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmqfxqpt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjuzhwmz.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gmisojmtq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gihajumcy.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gofowuxpl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gimqfdbpz.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeeybjyc.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjmuaakqm.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gjipfpody.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gfeszgumr.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhqbknab.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/glssbqind.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvxuizkl.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gmhegurmz.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gjgobvvgu.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gtximtwfh.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gaxurcwhs.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxinqoui.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqobelnet.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqeuomui.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/giwblacln.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqcdciar.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwcgtzmx.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/geymkvlvr.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gqtdgelkf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gcczkrjkf.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbgdchsk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gsvbirpnv.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsvhhpsg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/grdhtkmxu.sHtML


<!-- 参考信息 -->