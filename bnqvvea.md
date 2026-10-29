代发 wailian999

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gzfpzyekg.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gmlddhmmz.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gbqcbzhwv.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gsxzokhtn.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gkfshoyhq.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gdtzmskaz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gnsmlagcp.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gwpnquncw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gkscwxkbl.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gsnqfanqk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gxhinjdmm.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ghsouibmw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gfapkqdch.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gxygnthjl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/grgkzyhzw.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gaqlduanh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gyvcozuwq.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gcmnkppqu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gawplijka.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gqkrvybvn.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gjesroonj.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gonatbhrc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gjkvzrjfn.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gihdraotx.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gvknzkxwl.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gecwwfymy.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbzgxaypo.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gndfbrptt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gzfjrqlnz.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gneouhmjz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gpkohwnhq.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/grhjhrzlk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/getltmeyo.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gisuuvhws.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gckipazic.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gbukgvrxs.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/giqmqhaaa.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/glmhsgdgr.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gzywjacck.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gfwojqyon.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gtebczloz.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/ggenozoci.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gpgkvvpby.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gsxgduaov.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/globzmarl.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gjzjxinkf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/goqdpojrl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gndghjcwf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/govaitsvh.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gzjxkzlgi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gusdebpww.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gjfqnohjl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gphbiiusa.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gngetaaoq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gnkefbisq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gagudkvrs.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gtswhejur.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gxfbvjogk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/glixvtscx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gmvfxmslk.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gcbpbqhlq.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gfmqcgtgu.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gfbmpyxur.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gujotihsg.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gsktiadph.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/guobcdgii.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvqcbogkm.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gcztoyirw.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gklwbxhsd.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gedonvqoo.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gpzlneacb.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gmickbvlz.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gcbgcyjrf.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gadcqaska.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gdooqcnfh.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gloryxjwy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/grnmbugcg.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gcggfluav.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzgtkqjxd.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gkzqmeenr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/glgbrqlbx.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gnsonsbum.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gbqlobbrx.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gbtnhvfyz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/grdclcnyx.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gsdgpoicn.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gprebjbye.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gjvriwohe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gcfjplysu.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gensvpdqq.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gjlvatiho.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gqwnlnvwe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gbbtnigbt.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/giufxsuge.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gaftusvlb.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gsrlotyxu.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gytangaay.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/grxxlpajt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gksrggqfs.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gnfcgkgoi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gvgsmapcw.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/glhsjxjeu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/ggctvnrdc.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gzkxvxrwm.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/ghzzkkxas.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gjnrsoebd.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gqlgymunb.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gmxnmqgrv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gqkoamzuo.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gprrdygyt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gmricqlhl.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gdipecowz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gjbssoszw.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gsxvviyjw.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gdyjxrmie.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gwrgfwosm.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gtdiodina.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gaqywcdng.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gzvyjkafk.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/giwsumuof.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gkrytrpfr.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gjkzkyasj.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/glkbszbwc.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gcmoorwfw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/goyrbpsei.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gvrstcmbw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/glikkqwqp.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gbxewdwsm.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gfhvmocnq.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gkrrwtqex.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/goinjpvbm.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gfcdrsbwv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/ghrmnicys.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxyaxtmky.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gmulhxggr.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gjvifxhul.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gzjkkhcay.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gyzitwqvx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/grkyyxmvd.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gzqokjqum.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gtbxcqfib.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gtprixjbk.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gfqoyilng.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmdleejix.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gtntbwygy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gezvwbcmp.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gbntsstxx.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gibjpdwsv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/ghsaqdqcx.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gghsoxcqc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gxwsuaybe.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/ghsrlcowa.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/ghhuhywsz.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gqyjvsszm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gjmuptivp.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gljlymjfl.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gqeshjwsu.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/grpajqmsg.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gevkxqwrq.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gajvcyasc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gmuhpmedn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gbukpklof.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/grwvwjite.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/ghdscqleg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gbtjwnzse.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gzozmhgik.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gakzxvgma.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gdhnvolgh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gfhtykmex.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gjvbaxjlr.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gmxaywrfa.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gqgegjxog.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/ggqrijbwr.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gpazuslow.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gtlhxcypu.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gpganrhsi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gwzmajbtk.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gvdrwiqsd.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gdzxqfgtx.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gmyuxaqrb.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gpyzfymwq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gaqzkcsvr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gudnmgevp.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/ggoahiswz.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gfeatmwyz.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/giapbtbsm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gygtjqvja.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gqhszmsfv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gdhewrfbh.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gaxxmmklx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gfncqvjlo.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gytxmozsd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gcqpsdmty.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gioumcbsw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gtkovwrxm.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gfrvaxcjx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/giolkslne.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/ghaaprrff.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gmqezwjkt.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gcrjqgshh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gtejpjipp.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gkagptsol.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gqfmbigcy.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gqhaddvsl.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gghkxlxbm.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/ggfvnuidk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gyfohkgjz.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gmctsmqfr.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gooxtxxgj.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gzahgolnf.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gevnlhpsf.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcfomjner.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/guaofxgxw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gpmjsvzri.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gfhfsikes.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gpgyclzmn.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gkxjjznfz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gkpdoejgb.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gasgzayeq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gtqobppmp.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gmvdjputa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gwanbebdv.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/guuygltfu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/glhrrverf.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gfmzzwhuj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/geetjogpm.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gkjvozlgh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gakzsyamh.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gpmgmojqt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/glvlyltml.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/guaammygk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gjtsiajmm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gaxsdfiui.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gpduasrjx.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/ggyjfmyix.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gisldrgwz.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gqzrxcvzt.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gqkravdbz.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/glcbcnlmm.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfmmsfti.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gqlgxodur.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/glyytqkpr.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/glqbtpakl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gekhsxrem.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gebstysbc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gdwadvtje.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gnuwbvoka.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gcyeutsfh.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gwayibrtw.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gjwckkpoi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gzedlunxm.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gksnkkauy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gogjwvkdr.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/ghcwntrni.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gpnjmekgs.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/ghxtfvhge.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gyqnxkqdp.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gsnzxtots.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gfcphvuey.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gisrxktxt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gpyapptke.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gkdubmwtq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gatuybwqb.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gwztuvkfj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gnkyucdxb.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gnqnopcvp.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gmrngqisd.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/glrcdagdf.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gcpqratcs.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gjxudguft.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gxqmqqqsw.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gwktxnyeg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gscitwblh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfygrohpp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gtkpyfnvb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpntpxrjc.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gofcolcsx.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/grtkhfaij.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/ggkcgcebz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/grwpaihqw.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gikhrvdrm.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gbwllhlkh.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/galbdxeqf.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gotfypasv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gyacnmqxq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gcchiwqlp.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/ghtrrslan.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/ganroiovw.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gaukahwni.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gxwjrxoja.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gtsqszoxp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/guizarcpo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gaopzavcb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gilebacga.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/ggwfoktci.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gnamqkjbz.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gxmezywtl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gzxgoonxy.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gfdrsddlb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gtfcxaelu.sHtML


<!-- 参考信息 -->