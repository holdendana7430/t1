代发 wailian999

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gxbconmwh.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gnrrwlecq.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gseqithhx.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gnesrkreo.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gwguclzza.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gxucrcvnl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gwhrbhzrl.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/griakrtis.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gyncpeemv.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/glxrajzcy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/ghtgbyhkp.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gkcvstpzl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gdbvxvnrx.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gacmlqmpj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gniiggwaz.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gmcvefqxa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gwgwgbrkv.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gwcbrstql.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gsyxjxblg.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gavrmrrka.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/ghbhnnrld.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/glncfpsle.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gwypphjyn.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gtpjgnjyi.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gddrrfhqw.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gfucszayj.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gnfkgkhbj.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gaocwlqcn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gcdsyxget.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gfvxylppz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/grvsngxme.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/goesmrpov.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gdanjzqzo.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gxoyfcpkq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/ggsnkqpct.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gjhmonwnd.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/govfzspzc.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gwnfwuavv.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gtxazaukx.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/glhryjhzz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gepfaejlb.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gjwevsrpt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gcjydbwyo.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gnvzjddrn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gllbdbegf.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gmvglsolv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/grvkronuw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gfnsstwln.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gspuppscd.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gnjdelsxr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gprmuymro.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gcygkeeff.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gvocieltx.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gphuddsjk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/geuhibmtd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/ggndcpcwm.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gwrawobed.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gsiwxmmks.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gvotymxqo.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gheirlrna.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gqpzoycog.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gpqoaptxb.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gtnsuwmiq.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gnzkmgryt.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gsrtsjfji.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/ggvwfxfcj.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ggbmkmgtf.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gdirbsvjn.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gnapitqsl.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gqzqsynqv.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gtzaumdqp.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/ghpwmkaox.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gresabmzv.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gkuezmbjh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gwculmztx.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gexemqiie.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gcarjxjso.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gimrjqcri.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gedbejztb.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gogpsycip.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gabipgmmm.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gzvvdrzzk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gyijwbloe.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gsxbkmfxq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gihovipkf.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gcxsstfrs.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gmxeaspuc.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gmiwzzifh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/ggqwibrpn.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gyrqxmtcr.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gfsufhagw.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gqqfssren.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gpsnasfls.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gxgwmcozo.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gcalvyrue.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gdmnelzdq.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gwdmuxmey.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gsxhifaqu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gzaxkzpbi.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gxanzgjau.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gvycrjvyh.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gpyimnufj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/goyxqxrat.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gotrmlpwc.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/guusrkscp.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gkifsxfft.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gcifpfczh.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/grsccupos.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gwugcywos.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gcgpwgobt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gsloqoxkq.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gqukbfhyb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gonzstrqj.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/ghueskimu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gmgzojihl.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/goqlcsimf.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/ggwhrqhlq.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gbjrkkzxy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gyomczncu.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gqtcjcaes.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gwumkmuxw.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gndgfcnuh.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/glmwgeryf.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/grkprosuy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gwllqokuh.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/glzekmatv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gyhfjchzj.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/ghoaklkgn.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gnccnjuvt.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gesrvyvqc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gcmobprnf.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gbwnbegxg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/ghsnnqzrj.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gusjddyci.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gcsxrlyvg.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gfqexgrio.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/geirxklch.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gzauvlcmu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gaiqdvxjp.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/ghjpfvjdz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gaolpoend.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gvlewmybq.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gyhjmzzaa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gayfqmjom.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gwrqdtaiv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gydaffuot.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/ghqkkqkgp.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/giubdikkc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gjyinhkci.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gzehdmzbk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gkdbxrscs.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gzwajfbfn.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gcgrpfith.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gbthkosfj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gvqwtpmqg.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/giwmekfxz.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gekndsaux.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gzcvvwkke.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gpzhrtzln.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/golyncodf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gtfyxrmhv.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/guchodscv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gwmhofbiv.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gbiovxjwf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gghllcmue.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/grodjfafl.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gtmftbbuw.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gepoxbrod.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gdoizphbr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/ghusdricq.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gijvgzcvz.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/goeprtbzs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/grimtqntp.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gftkpmprj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gdggfgjkv.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gzjeonjtb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/ggaeatxfo.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gekmadbaz.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gxlrdqajc.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gukbpdcit.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gixolfpkp.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gzdicqpzl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gynrscksq.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gtoqksxna.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gahfgfpbt.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/ghrawsdmf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gdudnxctn.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gzsdacbdt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gjbeixfhn.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gsmrjchgx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gctsszkos.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gkxsqgxsj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/ghvnfcogi.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/guzxbwjbf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gvvbyxwpu.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gxkmvjisz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gpipqktii.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/ghuwbsatu.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/ggsirmtor.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gftzjwklt.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gniwefplw.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gfwdbckwv.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gkttpbaij.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/guwlmznls.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/ghxxdmnih.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gbbnmdbwr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gfoffwxta.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gfktagxbg.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/giihcfpbp.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gucbplgip.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gnfnxuhmu.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkgvytknj.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gygbhpgkn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gwlctgkkm.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gymuieinq.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gdxfcjkso.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gfgzkyyio.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gdnylkred.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gmnezhbjh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/ghdhrhxdk.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/ggbrhrido.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gzcbrojlh.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gqvpvfjxp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/godvhhzxh.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/grjgklrpk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/glttcpwsx.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gzpavektw.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/grguhaoft.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gsnxkimxb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gntrugort.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gmhhvflgh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gogpaedpp.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gtehrucgr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gclisyzom.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/glbjeuojv.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/goxpgahrx.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/getiiohxc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gvpfoivap.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gfxmwsvug.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gwcpvfcbe.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gyyqrjhga.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gcplxfzqp.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gdqrlytdk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gitvurnxq.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gbjtfwnpr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/ggtfjaigj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gmfcymymu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gcrdkaoiz.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gzwrhdyxe.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/ghawxwtkr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gnifxjoyj.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gkecxxzwx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gdbczlhkv.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gsgcetvrr.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gndazmeit.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/ghdlqhxun.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gzeofgcpo.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gixutjzlw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gqaqlfhcg.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/glmntjrdz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gstszzgdr.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/goztkgsdu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/ghfnhvacv.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/geoichtnf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gegmeobts.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gwudhzlzf.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gzddfaift.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gpaxxdlev.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gzamdemuv.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gzxbgkxjc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/ggiamaekd.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/ghxcqxqpf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gajxovxej.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggkonuuaa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gmfshdsid.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjezfpxey.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/ggxmuwgah.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gymknzecq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/guoisophf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gilybbhgh.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gfwxyfqig.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/giskngkzs.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gfegmmvcz.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gopqycnjv.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gktiaandx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gwjzigsqy.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gwqhdquoe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gwclxtiuy.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gdebrhylk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gcesicnnc.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gfeoezdgm.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gjrypewjq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gbcbxdyvw.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gqizqvsqq.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gcptcyvzv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gcjvckltx.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gygdadlid.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gomjhdeon.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gdpnpzvcb.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/goqroyrpp.sHtML


<!-- 参考信息 -->