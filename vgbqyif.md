代发 wailian999

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gsxiuwksi.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtaiipih.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmdtgwvu.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gzgqnsfvc.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoucqbmk.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcyzwqnt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/giunxutqp.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/grwwvhonq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvwyqyxyu.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gyirbbjdz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grdbaitor.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplllrpqp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrdpbpsx.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gcxfhjcwt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsnzoftp.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gmytkrrmf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnqnttdi.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gjclahrzn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnbjgxttx.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gsocxiocg.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/glrtumarh.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoyjbnsf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmwfwabwt.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhntteyk.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/genluoizz.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gjtikqhqp.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmrhbpyp.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/girpborgz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmcjzqhv.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gnpwynykl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/giepqehwq.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/ghvnjbhou.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaahnykrg.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxmyhfjj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gmbhtivoj.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/ggnpsathx.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gwqzqabvt.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfnopirf.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gttcdpymz.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdfqxlpf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvuaosmzb.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gzhgydxyt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/grgifnpht.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbrsgljm.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvemjdsj.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gfuiykkvy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjpwiwpyj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gtkbedqlb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gaqvtbvtk.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggikptjwg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gpxiyseyz.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gcswzgeba.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gihdujtkx.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gywhtxera.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnpvefbu.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/glqsjlfgx.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttjhxuig.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnxqgnqh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfpwncsf.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/grwjlfhjs.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/givmarnui.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gmqmmkilc.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/grzmgxjwp.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gqwoazyeo.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gabueyfff.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcetvcqu.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbztfnbx.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxfylouz.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotbldjvr.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gdupyokuu.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gfrmlrkdz.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnlxchud.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gntrpeznq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbifclrqn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeyoeuyr.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gyqozyulc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbivxjzmr.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gqjgdlnee.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqoladvzq.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjlypedm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbeyobdx.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprtvkphu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/guneyxltk.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gwrikexnc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gqpbghcco.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfglkroj.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzpuzrzit.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gapuycgnc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwbzvorx.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrpprhgx.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcwrnovp.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gixgkvnyi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvxojzjl.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gbxhrxeep.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvbcbwfl.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaproino.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwcddgja.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpubxjtz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gxmgywavz.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbfirabn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmmaxpvs.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gsiijhhlg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxzchmch.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gceakpqpr.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdzujjqm.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecbuivky.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gmxzwbdyz.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicperedz.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gurjmktgr.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gitbiowgf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkbkvvrc.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/guovrjztq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftfreumz.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gortxwbsj.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gefybulgb.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtvqibsf.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gufabggyk.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gfjhpzshw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoackitv.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwipoxzp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjlicolr.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvwtyyic.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gsixczmvg.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxcapyoh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gmmrhbwcu.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogezwagq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhpqnxss.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkgkvjoo.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gsubjgffm.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlhnnxpr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gthtwediy.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliujjlnz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/grvqwjsnx.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvdooiwtt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gimiehpje.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/greygvfna.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaixhrmv.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpysoebl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnhiommqr.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/giajukwzj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gygfmtlmk.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gycxokhew.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfliecje.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmuggaku.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guejbseey.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glngueeie.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxklafsfu.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gvjjenmag.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggatubkkb.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gahvmrajq.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbbobvoy.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gbmqaamqu.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gxfgzmtgd.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gsifpolvy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsirpszo.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsygmfqyl.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gletedsks.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/ghzdkchkl.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gtbxoqmdj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxubgtft.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezlufuzi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gucgejpvs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gbpmunmzu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrqnfiso.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhczugtd.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gbxwndhks.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyccddaq.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gycmypvis.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gxcryxxyj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/guvravirl.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/goaaegnnm.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrpxlqdf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrubppvq.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghqjiinbm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gajpjqtmk.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhifwgwr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gblhypcwa.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwfuxbln.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/ggqzfbzhl.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmuiibzz.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdgyfvjk.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gedthgiom.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfxriapg.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gocazwmjt.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gdmxixknq.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gliibozpp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzezzgay.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhncmrbd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gnlpcydgr.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gwwpqrurg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfydquzy.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvhdnhur.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzzouxfb.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gwizdehva.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gaqfumbkt.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gytomwecy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gfieaqziy.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzuuttab.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/grqxnwcai.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gfnezmyjv.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzddqocsp.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngsnkfqe.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwwdedtb.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdgbrgeae.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyyiedfl.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/galoszjjw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtmxdabj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhanxyic.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlchygpi.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gimnewjhy.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/giqkjnbmu.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glhrdxmyo.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gkznghurb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdpiveam.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gtbuvghwr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gflxaubbs.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/goeiutmml.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gomiinslq.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gmamhticx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkxpoitzt.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gubupuxyb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggycwonhw.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaxbslob.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glxgchtyj.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gtgsgizge.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdflmbrq.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gdijcjhtl.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gwucckqgb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwibrxnc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gmhqvumhx.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gbazjobtp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gaeaivdyt.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gawfiutmz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvjpwkqw.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqsylqvrh.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gieempiui.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gllfissru.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gklnnjdvu.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqrlxdwl.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzysrnid.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdfsrhjh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gmobxgifa.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/glxcpiebr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcvarpfhv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gjruikkxc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqyvsgsyz.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaspmiiig.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gvtnplaxz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gixypmjya.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gktvxrojb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghifznjyc.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqxjdgwo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gsuwvfqga.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvivfjdaj.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gydehvtci.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyyoewyq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlyqezry.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gabuxwnqj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/grysudewa.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gzgelfpuw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gpfftwtls.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxbilmlr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gqbqcokry.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gyassdeph.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtxklgca.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gtokqsejr.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqedxatg.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gyttcwwxl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqcgttkl.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gznvzbaen.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/ggvxzwjfo.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/goxydnxsb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gnpizpnnz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkknlzbow.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guevstfec.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gilxahybl.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gthqadjgq.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gbloojfcp.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/girfvamzk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gglgnyvfe.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gfbmvwqgt.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gippuhlck.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlgtujkj.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gjlfjjkul.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gfjxexxuq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqqcjuaz.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmmusfrt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqotyzbb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/ggazvyyap.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gegrkvqyx.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuyuxezz.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkyzjlyi.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glwhmzngr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwhqkszj.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/grnwtpoyc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gdieegppi.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvwchunt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/givclrsxa.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gytlilopv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkpznjfpe.sHtML


<!-- 参考信息 -->