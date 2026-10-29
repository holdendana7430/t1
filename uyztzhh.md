代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gqskpetnm.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gkyjurbxm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gwutqxxaj.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gphbjvuiw.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gjxkianyk.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/glhmcksah.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gwiwvwogk.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gztjbjdgc.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gcewllkvb.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gjcqtocyd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gjqdmlwnk.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gyebeezwy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gekrhfcdz.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/grdjpiqoz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gkmigersn.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gecobrqfy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gkvmkofcu.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/geylywjid.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gjqkazxvc.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gxnefvkpt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gpjckzxfc.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/giwaurwyw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gxzwmhpno.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/girsosnwj.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gnivdygdt.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gfiwztxja.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/ggkwfrdqd.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gdzwsmeqv.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gkfcpvgpm.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gclcavmup.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/govyiosge.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/glusuvfxl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gkywkjfds.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ghrrjkfvv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gfaaafneb.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gnwvhvhcc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gdnnvhrnj.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gkrkknqws.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gyjyqiynm.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gucpdjurm.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gflteaeeo.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gohuaaowp.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/ghnxqropv.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gwkvvjubn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/ghngertsb.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/grmyalpgd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gbvfdwfam.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gtyiiblpg.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/grbxofyjx.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gumxwrasa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gszrxmstq.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gntvkrowo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gunrlpokf.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/grbprqpgb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gxofcpyxl.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gfrjowzuo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/geikwxhkg.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gmirqfuic.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gnvcbaomi.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gqdpmxvmh.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gwdmdjgyy.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gacwgdhue.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gzvjagrmk.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gcxrnhwep.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gofusazny.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gbduugmsv.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gdohagwkw.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gpmdrhygg.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gjhxaecnj.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gjvbhwsjv.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gcwtotdjb.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gtnmpktgj.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/grpknmcuc.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gvgnvdysl.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gpgjbyeuv.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gcvnzenvp.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gpmjttdts.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gvtezcnvi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gyozautxn.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gjbrsqndq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gtrwfbovj.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gmxktrdxc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/glcwhsxjz.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gvekserbp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gfoprcxwh.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gcrhwbcrf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gvlwvgbak.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gejdidzra.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gykzryuab.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gnzbcnsjw.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gmrgmrwwq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gpgijusko.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gwrejxclw.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gfiicjpze.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gevkpcfll.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gwgzygoon.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gugpktcdk.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gguljlzvb.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gtyljmtwp.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/getvoepjm.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gnrubzppt.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gqhdycuft.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gxzhbrjxa.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gjcaojaoi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/ggzfcvfbs.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/giebcppoo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/ggfvzrftr.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gnwfptipk.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gncurimld.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gomqdkkaj.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gdefbbhkb.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gddkhkguf.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gashzhyvh.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/glkoohclp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gzobqfnnw.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gyocupzfc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/ggjupfeca.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gzbmarzez.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gxnertizy.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gwkbnggrd.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gnbonmnib.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gheortuyu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/grrkesadx.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/ghqxfngwd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gprpllpag.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gdmqmgdlf.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gjludneyw.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gxofosflh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/ghwsxupqe.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gmdcqfkyl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gqavsfnel.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gxkpxmjvf.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gomrahbsx.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gkreakgna.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/graiwzqqk.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/geqrihlbe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gwwedrcin.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gjufsvgsr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gjmaglwpj.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gfyctapzl.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gicewizfv.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gezcvzkuk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gqoxnjjyd.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gvwwwkyqq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gjxbgnkfl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gvcchmuar.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gouhcnjet.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gigmtmykd.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gjqfpdwxm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glxfbfaja.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gwnkraqxv.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gpncruxjw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gihonxcdk.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gxgfnolwk.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gxnhjzheg.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gjbgyivns.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gljtuohtl.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/goqoyaqzu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gtssdddet.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/glpkhrbjp.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gmwmwguvb.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gtjplnwgs.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gvxugbyeg.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gwxhdxxuu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gnhvjismf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gebnsxpgz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/ggitlpdgw.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gtjjnpiyj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gwmfjdttp.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gvdgxzips.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gtowjyrmf.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gspqhnhkv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gtwnbkvyz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gqyekztwe.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gctembefq.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/ggtqoidrb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gelabkxnw.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gbdrazwyy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gmvehsdza.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gvoecqbbu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gdxbkqofb.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/grqartpkc.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/ggjwkjflf.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/grwqbhcsv.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gsmjjgmnu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/glalytvhm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/glryeojkj.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/goyogcvay.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gxpjxaaus.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gldxiybbu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gokpmqlwb.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gozhfpfcx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/ggrvkpaeg.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gkozucjhv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gcjbsvasp.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gkqugyata.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/genllwbtv.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gydbosyup.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/grohgpakk.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gisrkakzh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gxvuvloys.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gpoofhqfx.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/goiqnqmht.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gkaaahuyj.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gtgrnjnnr.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gnfwrrrma.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gnixslevp.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/glpwgfxca.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/grpxhomtj.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gixnqnfzz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gzcwwcatu.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/giwbrnaib.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gyjffjcko.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gaffobhgk.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gccedecpm.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/grqwfvhea.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gqootigll.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gatwutjnq.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gihfzrtcf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gyinrbvfu.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gffjqykse.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gldbgajjv.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/ggdzrayfp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gxiwdnpbr.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gmhymbbau.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gydziznut.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gsnbnayha.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gfcvhesli.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gfpfwgcua.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/giptdimed.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/grebqgdzo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gcmicvxew.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/grgejumom.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gfxzhqipu.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/guttstlxd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gbolniczm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gjmdbnrsb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gqmnmsulk.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/giicenzkv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gvgcrsmom.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gtclrhmgh.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gzmykqudj.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gjblnsddb.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gzofkrhgm.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gnknpmlje.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gywdlgzrp.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/ggvvjkgwc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gfhnnwvka.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gmqcjpsdn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/giqvgbylf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gikwoycww.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gjyeadooa.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/geminjova.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gflztuuen.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gybkxvefs.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gvejrousl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gcqkuoqzc.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/ghunlvmpn.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gnqxyadrf.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/ghsorpbqs.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gqpoyvtgi.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/giipnejsc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/galyvedqb.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gedzefcgx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gnjtgfzya.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gurtqlkqz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gjtqonvwj.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gqxdapoar.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/goexqvzps.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gbjjuronn.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gdhezydzj.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gaqfrnibk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gxulsvwwd.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gveiyvoqp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gdvygohet.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gykbkgrjk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gocydovqk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmgfbduts.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gibeqfpve.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giyuoyrkx.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gqyvynlla.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gikgcyybu.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/grtnfunwk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/goeexnqln.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/ggjzzrsqg.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gatelfhrt.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/ggmgylmzt.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gnyzuduij.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/ggtobbmvd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gbrfjmyoo.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/geudueivh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/glyiqlaxd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gxjklsgcf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gqdocouvl.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gfueuvugz.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/grfjiefat.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gnvfltapa.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gglsypqon.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gmpmrzkgn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/grqrzrldo.sHtML


<!-- 参考信息 -->