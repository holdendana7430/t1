代发 wailian999

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gfndchwib.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gpqcbrdsw.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gxxzqnewr.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gewmiwyln.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gbmikahma.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gtkfxsokz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gkrtzfovq.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gqnspugbc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gknshkwvk.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gcstgpdwh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gqgxvjhqf.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gauagsiqd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/ghuaybpqd.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gcqylpsln.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gbpnklqby.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gyhybkkqn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gpptxkjhq.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gmootvenb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/ggnmbreut.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gbclkisym.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gdansausb.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/giqhkvtma.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gusbrshvz.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gidhupauk.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gmvmzhdej.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/goorqgnzy.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/giwiefuan.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gwftsosqb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gprfycueg.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gjbftbcnt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gkztreiza.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gcmhurqkw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gxurbltvq.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gdiuwwiji.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gnbcjvlrs.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gokgfvtwm.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gpzebpqez.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gnylenosp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gkpzgvcrm.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/goyhmsztr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gavagjjvi.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/ghtcmukhj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/geqknkwta.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gkuvljxuu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbxjirrfv.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gussdruza.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gkrlpplhm.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/ggqndryme.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gkasvlagy.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gelemknls.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gkgeososw.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gwsobrubt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gvsqzxwmo.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/goifolsqp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gyptlmaty.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gzxkfyzbm.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gwrhjpfeg.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gumnnopcw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gulhffesf.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gixqhvagg.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/goiuulwkp.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gpzcuulpj.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/grjbizdow.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gxphtfdya.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/ggocjiyzj.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gemrqnmlt.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gypflotba.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gvtxlmoub.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/glaadpnda.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gtjcemvau.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/glhgaryxs.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gtuktscqd.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gimkbjohy.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gaploinli.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/ggjpmytrk.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gniurxgpr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gsgnusofy.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gxwhrhven.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gkzzvtcyp.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/goaartmge.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gyehysvaw.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gfcnmojrx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gwndqruoi.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/ggecctqwp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/ggueaapwr.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gvpakmccc.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gbeavlyby.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gtjgcjstb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gkwkqrpks.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gccbtwrmt.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gzlrtwavn.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/glcdsymwt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gbuxdjuoy.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/grktagosf.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gjaayekda.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/ghobwdeaj.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gqkawnbbw.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gpnnmzzyl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gnkvseeex.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gxygybzch.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gogleqycm.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gjejwxuou.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gkypppjzb.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gwmpwkrix.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gzhikngai.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gezaplwaf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/guoruhhqo.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gettbrvcj.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gdrlijqii.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gtjmofvdl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gvavzlurx.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/guzgbcrhh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gnckxzkvv.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gcbwybyyg.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/giuwnqzhy.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gvuhbudho.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/glhwbpjpv.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gdgfamrue.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gbxxbfvul.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gnobuzjrv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gcuoanxlo.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/ghpngmvrd.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gvtbqkwps.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gnuhjryob.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/grnwebpjb.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gplcuxhmy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/guniqetik.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gytwdmobu.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gsdiqeane.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gfbntbxas.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gckgvmiqs.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gqxytqzdn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gelpeyytz.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gsaljjtau.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/glhspsxxd.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gwhdhlezn.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gjycpcmjn.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gipzpdiin.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/ggazfyprv.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gkrvigqgt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gdtjkfpyj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gurekjnik.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gfgsittby.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gofeijllk.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gekysplaq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvnwjktmm.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gnfuulmoa.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gcyfpvcar.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/ghlwgjmnl.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gzwbhpafl.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gnhmwdrss.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gqpadsqol.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gfbhybaxi.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/grkxfcxno.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/glruvkrih.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gsztvavsc.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gegatkbwb.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gjwjjohvs.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gmwwtxcjc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/geynosbel.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gcauaijqr.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gdallycex.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gkpkrginb.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gjzxkaldj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gqlzssjep.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gvbwxfsyl.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gntdmsrgt.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gjwnzyagx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gqyxsnfpw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gjrbcqhmn.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gfyhtqhxy.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gxpjudbsq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gmwhieojz.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gukzylvrc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gyjjakvvh.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gynlgmoqx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gtvpqzcjx.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gcabkhqrg.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gfwhjqujb.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gxngmynrh.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/ghzlldtpr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gavqicaew.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gvujmjszt.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gynvpoifi.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gubcfklau.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gdhvoowxh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gfeyrdpva.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gthnsxhgk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gfdilxovy.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gzczyuznw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gznomtbtr.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gtozeqqga.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gjuvgyhwx.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gqjnckkls.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gsimqdieh.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/guauggqzh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gwikyrelt.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gdoevxcaz.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/ghrqvnfrs.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/grcxbdttt.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gsvvrlrov.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gkmozufoh.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ghkluznxv.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gzwguaszy.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gdcfsyukr.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gtsxuxgqw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gyockikjc.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gyexgtudm.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gdxrqysth.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gfgbbaaau.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/ghihosdaw.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gasrpxuhl.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gpvykphca.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gjcmbeuqw.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gsstyncmk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gxdhegivo.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gytbjzmcs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/glcyqtkws.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gnsxzamom.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gorletobk.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gxhvewysy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gyadjfcoc.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/grcxqymbv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gidrbqxvg.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/geiglczie.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gtcpgkawx.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gujcyijpo.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gbojfehtp.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gcjfmzrab.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gaikzucaa.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/ghsmtvswt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gpkubvppq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/grsivnnte.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gazctcosr.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gdxemmrkh.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/ghrxlzeiy.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gmxosswab.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gxmhadtoe.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gsjoxjheo.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gdnztsbej.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gwbphvdvv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/goyjeehmi.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gfvwjuerp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/ghiykvimn.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/guxbohxse.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/glvpsifkt.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzmywzprw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gngurvlma.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gsafjbdrb.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/glbzovniq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/grigvpmvd.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gtwwqmwxt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/guwozadyf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gmqupinem.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gnpsxdgga.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gfpsoqwva.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gjqnagygz.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gjxnledeu.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gihhhsimk.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gebyqpgzn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gzbuvfkos.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gazzhjvoi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gytjlocnt.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gzbrfexae.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gmyhlnjkb.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gagqmxjne.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gnphdkpaj.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gpbsmbvac.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gwkudgvtw.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gvxrrztft.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gmriucoet.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gjwrdiwdc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gdhthpeef.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gniesglty.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/guzaismwe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guzkjhhuy.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdspozaqz.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gnsacoisp.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/ggdhynvov.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gaworvgwv.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/ggrdygjxi.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/ggexafnrw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gfljtbzgl.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gjianirsu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gchgrwbol.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/ggwhqpfud.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gvwrzazqf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gnmawjxxv.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gcffsohlo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gqdsmpzdj.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gourkxzrr.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gypyfpcgu.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gfvrplngx.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gsaycwamq.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/ggoujidyg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gaglwjfet.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gmaiamolh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gsxjvwxvm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gmdhxhatt.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gsnzfwmci.sHtML


<!-- 参考信息 -->