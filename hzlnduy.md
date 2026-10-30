代发 wailian999

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwqtlzxvr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghirusvxf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxngeras.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glhwkoijv.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnevfcbnp.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxlrlxcj.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmflvexuz.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grjvcjaaa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gyukpavcd.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcknrzpfa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gymipznwj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gvbxasgro.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gabdfnyht.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrzistvl.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gwkfblhum.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqmrroet.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gocuagtqg.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gtpaznjqb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohfimaqu.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gezawuqhb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavgqtrhz.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/grldtisrg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghllvrdzv.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/glovilwko.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsdlpwuj.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxjqgaad.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtvflosg.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gqwdvikuy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmigrgxgs.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gkzhjjala.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/geampfqin.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geposokfo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/getdxbelo.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyzhclmk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gotwztcpy.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gghuyjeqo.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtrxtajht.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgicskgj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhswwrmb.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gexnojrmd.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqoyvgfr.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gnzakkxri.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/goeklhrep.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gdfhyoeob.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyyxosgi.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykdydcxu.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gooafnwcj.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtyqcduf.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnwiwfis.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxqeuyir.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gaesbaqsg.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/glnjennks.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gaourhgyb.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmpvqozi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmtahapo.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyqbeqtex.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeugsglz.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/glwkbsbes.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvubqsev.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbixgeugt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjrjyazy.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gbglkmqyu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdghusqaw.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gmgadbyhh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gzclcyiwq.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcatluvw.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwtjbkeza.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfguedlys.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwyeysam.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmitmbyab.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxjlxmsj.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gkareklws.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthsymsmv.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghozyzqnz.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gihtiafgu.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsiurtpm.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzbfklbc.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntiowzyn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnkigxco.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzttwyln.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gtxwbefsi.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gshgybhvd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/grtkzvdep.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gkkgjiqzt.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkcfczsn.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghudxaxiz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gptxwkapw.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gphvdopod.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgpntlvs.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gsbhtjnux.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztvzfeqg.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuxgbkfq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gablnomad.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxrxyjiu.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gywpvdaoq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmhjqhop.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gtgswctpj.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwmrulls.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskhsduya.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gapvtlbag.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrvwbuhn.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/ggrltefvp.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gohmdflxn.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gukfzkqvi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/ggblgdjtb.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/glicwutbg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbrtsdoy.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gpfsnbkqo.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gubszexrx.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/glapllblb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grmvpqgku.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvormqprs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gyzbuxjkc.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpzdwcxas.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gowuectjd.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdlegfxr.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/guihkbxxz.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaglgxjg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpulcvhc.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/grewrtsbt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gloykoijc.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gfonvjchm.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/grmrwfmvq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gawuarfxe.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqyzujag.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gggivissw.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gyinzznoe.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmipbwjfs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmrctbipg.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gnligxmoc.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxmewmxs.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gprlnymyh.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goztcxqzy.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnqiaaoo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/glmxopyye.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmhehjxqt.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvaufgqx.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoatxhjt.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gpqvpuzln.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrwvswji.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnyzavrw.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/grhuutxww.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbjgozsw.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvuokaak.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gwhsenitf.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/geyzbuwib.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkotsuneo.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmljcgxyx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgxdhfeo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/guqydhrhx.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gqrjtrquf.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpvdnbudd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpziteidi.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbwjucwn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gnfrspwke.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gnptmklmj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gbfaankdq.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyluegij.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gyihrnzsn.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmguaiuq.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwtreaqq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkmcqpqr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/glhwfvfhn.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/grmbkgkav.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gkouaylea.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcceljmu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkozyvsot.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gexifmttk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzscyvhe.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gnfurneel.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmlyxbae.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gimdrjdxi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsnnptge.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwduspaw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqdggmay.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxufxpjr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziauawiq.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/glopigtvq.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwarizoib.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvwcgqoy.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gxubroato.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gloddbifr.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkhynbdx.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfxdliqz.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/glvxnygaq.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizldzrdm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gifcrcwwr.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbttdijy.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxabuwoq.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gxrgteoym.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gplrfgywx.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gyajwzpnp.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhleetcq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnaflisf.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gmcygqzib.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnozeerx.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcvhxhts.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjafeeoex.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrjgarnq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqihzzxc.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gleadnbwt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsonqqbkv.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gncdiyndy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/geqkakyrb.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrhyiwsj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gbqpwddka.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/garsltzzk.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gxktyvggd.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnxajkwy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/ghddfuleh.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/grjjjucjz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswsqzxub.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gidhfntae.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfogdkns.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkonujao.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gaulmfzxv.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gyjwpbvlq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbcbuhlu.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzbyvvij.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gucyssntc.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/ghainolis.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiyxduvj.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsvwttog.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpftvfuhk.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gnjzeaddc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwwovqaj.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmceaeykg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gkxrajmld.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/grhxclbhd.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gncnmmncw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gdvqlkaav.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gtcvxrkkq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gqfhfdlnb.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gceehosjt.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gklpxcgge.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqndvnri.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggujximdn.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gypapkvjf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjreiaqd.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqggjaen.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnmkszbq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/guxcefssk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvsxkejg.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdedkolkr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gghhtfqis.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdepqbnkh.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwxfrpoa.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gasycoics.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/giqqisdgh.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gjzwftzkk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gbuvvyptk.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/getpqmihc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gvnjgtnnp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazevhtet.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gzgicxeqq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdrblmih.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvyyngssk.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhwmamug.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbdscdgib.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gzfmxmfgj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/guapxppbe.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfjdihho.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gxhwtdvse.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gertbgsid.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjegfycaz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gbvpvzbsm.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpqcwxrh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavykxlnb.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/guotbwqzi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoiaebwt.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gtsdtfjza.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkwbygct.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtdgjgom.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gfounclpl.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/guggymchi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gxoldxfyn.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/ggzfkwmui.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gjktyxbrj.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnglssnv.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/goxpwvtiu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffhahpqf.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsebpcxmh.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvlxwing.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdigwzdhv.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gmdjfspir.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gzwiknpts.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gysdqopyd.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gpwadjkgw.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpejjjjdo.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gqsbxtahw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdfseeuw.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gtsvymedx.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gglwfbvhd.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuiwxjtb.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgkfgnyu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvxeuyuj.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gklmslpfo.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaidtdws.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/giciylvky.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnykbsxdr.sHtML


<!-- 参考信息 -->