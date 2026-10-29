代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/glpqmppoc.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gnninnvwr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gblmmxhpq.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gifwslzay.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gvgpxyfqe.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gwrcjvazu.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gzodhsjtq.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gzmaztkmc.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/glzpbhylf.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gpfcjmzlj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gfdjvcgti.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/ggecelnra.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gscukassb.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gqhwhpffl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/ggszywnss.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gwfosnhdu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gwvilkoba.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gwajacezl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbtpkduiy.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/giidgwlie.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gjcourzzi.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gjgrckssy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/geigipbvc.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/guudrslzu.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gkzzbiodz.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gfgsqbbpb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gzegcckau.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gqjnekaci.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/giodzmthq.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gpeikzbhr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gsbreuyfw.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/ghkyiaire.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gmiexqkox.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gkseofzli.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gwasgrtas.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gjlgdxxsp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gbjvinnna.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gcaarkcey.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gbpkpggeo.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gdatfmdye.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gfgfhvdfo.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gkerdbhty.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gfitlnjbr.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gjmipobhe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gkhlxawjy.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gtbkgzpen.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gdoikhvno.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gegrmjaso.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gsupemvwt.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/geshjdcew.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gzruueqnz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gtrkxgjle.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gbcywltui.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gfvdngkkp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gwaogfhsr.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/glkqegfeg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/giwgxnvko.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/glnwqwogl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/glpthagwj.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/guaxfhmfo.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gblztqybg.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/goqyzegwh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gydiinmpf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gcpsxicjo.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gzvfxagyb.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gnuhtzsqt.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gdcghvbxb.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gtukenrhf.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gggkjbvnh.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gvkkzsocp.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gngaxisoq.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gadgmtoso.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gmnxgabam.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gjpjssavn.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gkgsglsvt.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gzaiohbrc.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gaeodsfon.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gqxzyaxqm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gabwzznip.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gvmbcfawo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gnbbbktmo.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gzrhufvcw.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gghxnfhmk.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gmdttmtws.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gircbztjh.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gfpbdwujv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gqulonmnz.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gczogdpmb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gdnzcefcv.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gvmcieiyl.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gowieibpg.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gcdgsmylu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gsvjqyorh.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gmpfsnsoo.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/grvguyyqy.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gbnyussib.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gcycnfrnv.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gjaluqamy.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gdfphhsld.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/guovoerhj.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gnnqgdkor.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/glqbtvagd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gwiemryvk.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gxqipjeuo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gmsaoaqux.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gcrffmbrm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/geoadjvma.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gbzkcjrmb.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gwpldkras.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gwxjmtcqi.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gnhotfypp.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gcloghlnh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gkbbbsjmi.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gpldtjapl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gsijvpaot.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gxzmeifhn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gypjpmgpq.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/guafycswi.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gepbggboa.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gfewpkqlj.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gqsdrrvse.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gkwjvedzs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gzdgsnjyd.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/grabtcocr.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gzcdmweed.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gxlkjbaft.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gcktrzysm.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gtztyfyxg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gcavlmxqs.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gqfcpxdol.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gvvznzswi.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gevblutwp.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gehzpuuvy.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gvtxlossh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gbwwphlho.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gnthiputw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gqvivvgnc.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gqmkdnasi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gcmlfafhm.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gdncwseoa.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gktpbslsr.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gxankkwwd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gzbtxadti.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gjigrbepv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/giehbjirq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gpqzwrgrl.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gilriihzl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkrtttifw.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gvjqkffte.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glybhrxue.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/glmtvvhaq.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gogjxagxn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtztuhptl.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/giqrutoan.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/geaoevhva.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gjhebdkcn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gicaptxfs.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gmcbezgoa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gtchdwlyu.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gmjmmzgxf.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gkqrwoxpv.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gmkkljbuv.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gzvwrfafa.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gbnopoezd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gmqybvwsb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gkdsjypjk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gzdkrywls.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gtyrwtgry.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gyxklqrto.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gbywmuqvp.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gjctrjioz.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/geobedkya.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gdqwjikit.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/grciujkax.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/goafgtfcx.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gzjlocqll.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gciugjyxf.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gzdrtsdct.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gphlsevar.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/grmsjpqnl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/ggzbzevfa.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/ggthrfuvw.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gipdhzpre.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gabiudzsx.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gmneovtbg.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gdalkyxlz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gkkrwatsl.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gghvxbppd.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gymhakqoa.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gmzxcqjts.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/ggioiavsp.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gfnwttjyu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gxrtmitdt.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gembszwbb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/ggchglmhx.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gxwfkvhbm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gcqjiyrky.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gyhrjemcb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gaxnruuqn.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gcdqyvijh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gmdypmbib.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gclkgoabc.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gkcptxaop.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gobilclgo.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gltbbongw.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/goddorces.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gjokayqnp.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gruowrxow.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gbxoiwxhe.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gkfrbeikf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gbnlxorvi.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gomvmrirp.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/glchvamwi.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gxmusihii.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gdpjgqbiz.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gzzawzdoh.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/ghafcgweb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/grkdmvuhv.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gioqigntc.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gtrcpmkfr.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gktmtdhah.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gdtbktslg.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gnbcrvzjv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/griwuqecs.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gdopuqepj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gxsexvefv.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gslxamijk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gertijtfg.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gltdggbay.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gkdldlqbu.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gbjtibjfm.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gbeblhezs.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gvsdyfblj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gyffumyrn.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gpcoaqscf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gkauprced.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gukwnvxkh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/giuxhllls.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gdsajygfp.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gunmukqqj.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/ggeygnjdl.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/givbcssaj.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gbtjgtcer.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gvqvzgtyd.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gzzlhxfzc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gcfgoglhp.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gbwppkdiw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gratmjhkj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gypvslite.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gitauenmc.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gyhdfcfyo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gfzabhslq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gvbuoaiud.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/ggfmsxyou.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gfvckyosp.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/glwvbybxq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gjmsqzddv.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gjgawenxh.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gbfybloxy.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gqfkcoddd.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gaeldanza.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gzstizogo.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gwlaewsdd.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gtsiamdep.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gumvxovqx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/ghxacgscy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gsfdilodq.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/ggjrwoyfh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gadpnfgqi.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/giitvsieq.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gdmpiglcu.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gbhmnxpvq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gdxtjxohg.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/glrryzhki.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/guzcfmelb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gbkblqqna.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gclqbsnts.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gprlqtuvk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gfqysloqw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghzgkaodr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gkpkhklwx.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gmypoplso.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gditjdnji.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gbgavifgi.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gkyowwobd.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gxipjxfni.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gwslzihlc.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/glscmlnry.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gpcnjkmfg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gquwrqnoz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/glcjkxxde.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/goropunvj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gzqioaxey.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gbunmmddl.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gkvbznwyd.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gyhuzmoci.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gwsoalvwn.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gbpxmfimh.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gbhncazym.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gmsvpqwfe.sHtML


<!-- 参考信息 -->