代发 wailian999

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gnkvdwmjj.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gpdoezyjq.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gwfkjfljk.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gcbvjyoyd.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gxicilmtv.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/guxjkehni.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gvbyhemjt.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gcdaihqpo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gqgfryvbt.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/glisdurlh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gdtemwxgt.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/getjshnds.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gwjppbftz.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gkpufvjwh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gfuylaipf.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/galfenjma.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/ggzkapsuj.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gqybkcpqo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/glswvuxye.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gxolvlvsy.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/glmskieab.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gopivcrfv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gvixpvtsf.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gyjzuxpfd.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gmifwvklv.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/givqowzxo.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/ggvuaatvk.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gmgxdqgjy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gpqksjtsw.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gcpeqglbi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/geusklfbz.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gkfbandkx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/ghqnwfudj.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gigikdbzq.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gwaoccqmr.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gqegcwipc.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gnfppkgoz.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gwivtkpny.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gukcefpow.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gfomqqfto.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gcpnzvckp.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gomvnukci.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/grvctogct.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gmcgcbrmq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gjnosyjcr.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gxidoaqlr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gahgtbthw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gxprnsuka.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gddoxsawx.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gaxohgovb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gcugfcrjz.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gipgiuwgh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gjmcjmwmv.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/godyelswb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/ggjrvnaxm.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggmjuzips.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gwbndsrgf.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gqvgauwdo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gheotkqfu.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/geeqdrduw.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gpshaeesm.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gdgtursey.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gzulxqwvx.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/glzslggrk.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gvztaozky.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gxkyhyyaa.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gkwrjflbm.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gvtkffkio.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gateuytik.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gqmmlzwnl.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gwomsqofm.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gtccsudhc.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gzzmfpson.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gcjextrnf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/glnduesgt.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/ghkdjapxk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gzpftpamt.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gjjsgdduw.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/glwrrkcvl.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gvghtzynv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gbwhlwyor.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gbftptakg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gvojjdcoe.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gnwyimezc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gdnzeohas.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gurgpuuvd.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gkihrwdkb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gpyasbwqf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gtncdwgil.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gljrdttdg.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gpuluieeq.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/glbgwhljb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/grnregoiu.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gcacpvqdy.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gxfmysrkd.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gqppczylf.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gjkbvnrai.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gmnaktxmu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gxeaduqgo.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gbfnnrtih.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gowuzvgtg.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/glnthcbrm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gdvbrnvps.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gxreoenpp.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gvivkidml.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gsyrjajhk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/guevhdovw.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gqovwgsil.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gkvmcgqwy.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gszhusztz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gpzwvczsi.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/ghldrpmhf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gpccqpvtx.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gtedeyfzx.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gramoxeyy.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gwagmaewb.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gahhozzvb.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gwkcxngqt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gzaramxuz.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/ggzgjvjxq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gbvavyedc.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gkbchnjjs.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gywuzqzsl.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gnahprmcn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gtdenwjcy.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gyrkxdbsy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/grrczycad.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gtkcesojv.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/glseaskvv.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gmqxrezhp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gwhpghngf.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gbqevnrxq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gntpjjfkt.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gyitmssxb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/glhnzdpag.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gkfxsmgoq.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/glphigtpk.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/ghwwertrw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gtbkasqrz.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/glspfvwco.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/guukjxfgs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gxaqzpopa.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gdqpzgppe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjyddagne.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/ghjumcdkw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvjnwppnw.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gzzbsveyz.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gkyrdqotw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gzzyjsfrr.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gjcsvurhi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gwtuzsoxw.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gtdemnyvb.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gocdavqsl.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gembzjeop.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gaqjvfosw.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/ggcejyfzt.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/ggnulbvwo.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gnxtdresa.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gsnluckmm.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gbrsmlupn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gxytqsxvy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gxiiqcswx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/geruqezxs.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gpdpiuqwd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gbyxqziba.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gwaaekdkr.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gvwsjjfum.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gmbyrszzx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gaqjxequp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gszggczgk.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gupgzqtpq.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/giscgvvsm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/ghgfxjovl.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/ganwrvghe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gwpvnttre.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gmgacjcyp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gcxoenjeu.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gqmjyldjf.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/grwkfdgim.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gpvukjmgr.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gtiubdfei.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gynfgonlj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/groimlqsg.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gnrdrbkbr.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gguronjko.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/geuwnwxhx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gnvkjajro.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/grrswpoln.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gglluiatx.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gyhefottr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gjmkyvfqu.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/grlujyfug.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gvxyfrmdq.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gvaeaqgbh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gpoobffcn.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gveupxdsv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gijvzimto.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gefydygoo.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gzzqxfaht.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/glpxljsri.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gufjtafvz.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/ghpnluhqt.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gelpsuoed.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gkelihxmp.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gotfhfjfw.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gpfvujvko.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gkrpcmeqa.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gagjqhmcb.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gtigzoora.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gevwoxnzc.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/ggmnnrpvc.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqcehytnu.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/geahktqsj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gxboyfhal.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gqtecowlj.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gokxokkyb.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gvxjhtwte.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gyfpsnyvd.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gsjloihdm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gllxwdeno.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gwvrrlusv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gyckbhvxd.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gxdefwqfo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/ggchnchwb.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gdkmvlqwa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/geuizhztx.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gslpnarhj.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gtlcuxkpu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gveyartld.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/ginmfmqwn.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gudhnarlh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gsljrxjwd.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/ggsfpwhaw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/guvnpobzm.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/glynvkyyz.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gmjdpoglz.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gcpvlqorl.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gavhvaqvo.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gjyvvjxjo.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gfhaisipv.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/ggwzxubeo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/ggvazjcxj.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gjslnoptv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gbdpodxtt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/givsxpaag.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gfatrhmcm.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gqbmyltov.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gexqxtfee.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gwikdvrdc.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gyvfhvnkt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gmdbjzpua.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gblagatyv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gmpdbrxsw.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gjydzcqbu.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gifhqsowv.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gbsfkmsht.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/galawzjvr.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gpmokvqfk.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gxaglhzmy.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gdebqybxo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gtwymzcta.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/giovlkccx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gjcjqojjj.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gbxoaxmyd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/glowxlpfj.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gstbsjaqp.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gtfxlwygg.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/grdixismw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gapksnbia.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/grdxznjca.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gtegzwqpw.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gvfgvqxuf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gamqbwsrp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdvcuylbi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gqvuindan.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmqxluvky.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gurfwktfy.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gcsvhckbu.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gdicfoxkp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gfazfujvm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/glpepsvju.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gdqasgrtz.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gzocnijiu.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggofotxft.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gmyqpsdvl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/geuzvnvto.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gikjibplr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/givqrpmkd.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gkhkrthhk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gwpymcxdj.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gguwviplv.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gkeelmbav.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gfppixqpf.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/grrkxifuf.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gkjhewdzr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gohzsfhru.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gtfcogltm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gcpihknnn.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/glavxhjzb.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gvpkeosez.sHtML


<!-- 参考信息 -->