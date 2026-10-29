代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gymagjsxh.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gbwcpjjvu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gfcmhnlvc.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/geniivfzp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gbkermlla.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/grcqlduzs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gflqilebi.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gebmuvupl.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gdublsick.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gwmerzdog.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/guvnauilz.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/giqjnfmrr.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gcfhyxmmj.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gfktmliyl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/goduofyzc.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gxqxlqvwk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/glnwagjrs.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gttecblju.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/glmkgwuvf.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gskfjiwjq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gdnwzfnzj.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gyhkpggjc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gmikjejan.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gbnkqbfdk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gzfodtdtw.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gdfojaguu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gudxlxrat.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gzulxzojf.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gkanzttjc.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gpscnvghx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gcysvcslh.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gxbecbwuo.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gdndxncfk.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gtnxjgbof.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gkoxqkvra.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gvsgtpwow.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gbfflpvoi.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gdbrezllh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gncgudllb.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gywvehtqr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gjpqrfyxu.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gflelruue.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gagvucohh.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gqgzihuws.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gchsdgyso.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gnbntmyqd.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gzdizxqkc.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gscdrspsf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gsytripyn.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gnnzoiqus.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gvivzuadf.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gakilebkn.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gpresbmhb.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gxwolrbqm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gbmlekrvi.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gmujqlrvh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gqptonxzy.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gcxptpzfn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gpczgehrz.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gmvjsifdc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gxkaktwwc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gkjksrwmv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gnktyvltv.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/glfjiwcfx.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/geywmmvmx.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gnwrcfrlb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gcccqozur.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gycrvvwwj.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/ggqlqyozm.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gssqubiaq.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gwbixcwsp.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gllkuxdlq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gyubpfbhd.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gnyflagwg.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gizzipspp.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gusitquuq.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gmdbubaix.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gcwougvyq.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/grnxvtfhx.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gbrisucet.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gapzcsmyi.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gptzumxls.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gazxacryt.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gtcztmspq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvjunenwk.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gkaoatjtw.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gzkjnsrch.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjgpzkxzz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gsklkecwn.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gootmtlui.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gssowjujl.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gtmrirrsa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gyhsiyvwn.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/guizccsnj.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghlycastw.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gewxyrmjh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gfzpgapib.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gorzdrrxz.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gltfrgkaz.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gpmaxlcid.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gbqzaamkj.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/glmikbqqp.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/ghcujbslq.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gyopgcbpx.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gnlzugvqx.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/ghpbfwhbe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gnixkgedr.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gygvndbde.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gnypwppsh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gnqgefaad.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gvqakefdf.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gpsiaiehz.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gqvnwqjxa.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gvdodjajg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gbefstmes.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/grzucbfno.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gjpfdqxee.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/guqgdkehl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gvwswhrlm.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gpvhzeffa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gypovsozb.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/glreblqsc.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gwpfnfetc.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gbpsmopdx.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gpnyuxbhf.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gsnggzpmy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/ggavufbqi.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gnyeukhei.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gcqjcjbbw.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gnbjebhkh.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/geeqmmawk.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gsbdmussg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/ggdbkenfn.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gwadymbul.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gzieecmen.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gxqmyxmfg.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gpxptvzvw.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gxnqywsvw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gtoewendb.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gtzyjctqr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gershaxus.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gydlknhsu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/goalnyhei.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/ghduwcqzs.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gkijfnzmf.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gfadlboaa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gocylgnip.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gyepllare.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gekhbpsco.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gqziyzbhd.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gbqahckxi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzzfcjspf.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gpuurssox.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/garwlpuyk.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gmlupzory.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gkotxbpfa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gqlnkpaqq.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gfxagsuug.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/grflubhiw.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/goqwszeux.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gdbtavffi.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gjtwmualv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gylzvepdl.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gattanaar.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/guyokthij.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gimjtdstl.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/grtzwpubg.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gldxjsvly.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gflrvanmd.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gaicwejmb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gsgjhmtfz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gdbnwhzkq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gnyvgrcwq.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gdsojeebw.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gcuszblio.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gbwataugt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/ghaetgeey.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gvrggnkco.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gbomnbhvx.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gwmieiiaj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/ghqrzmfup.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gywccubnh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/grcybymhf.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gavddjjlz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gipofdfey.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/grhbpssvc.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gpcxlhzuy.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gclxicvzu.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gescwpfuh.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gdwztffnf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gsdyyhvni.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gsqmljmmj.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gzagedhxn.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gesrbgelk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/ggeidirzv.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gvinsemsy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gosjymvna.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gdbbhnpyz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gozamjylm.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gfplcngic.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gjabaylqq.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gteimugir.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gzszyesgz.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gfwudawlk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gvymecoaj.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gaxxmauzs.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gfhnneqcd.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gxgvgwbpa.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gruwvfcex.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gbftolvxd.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gwmulgoon.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gqfnnvfsl.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gjmoungbf.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gkscqnkeq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gdvscwzkw.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gjtwqvbzz.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gkifygxqn.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gpfppjljh.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gehrbsjai.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkdontibe.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gqtecbydz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gzeunxhop.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gelpiepcu.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gmbnknoie.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gnwchuxdk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gsjkumgdd.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gciupupph.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gpcfxqlge.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gxhfqcytt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gqqrpmrog.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gynetrbnl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gryitreif.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gjrssoucn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gzocebhsv.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gltqbkcig.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gfjwyczot.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gwfkdzopq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gqydjnbtn.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gfgkbyatf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gawrgvuhr.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gvuesxlfx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gswrwwhbh.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gzcccejkl.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gxgnbgfal.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/glklemnan.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gnflylntg.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/ghdtsapnm.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/giapsopiv.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gzwdwdmxi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/giiqyvdet.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gbtkpvjml.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gsaljmygd.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/getacdymz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gseskaemn.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gyqxqnxvy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gxgqxwzry.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/genmqcvgq.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gvrcnkekv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gijjznump.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gjllhajmg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/guwdhufam.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gxrmzbmlb.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gfyizybyt.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gtcjjwjzz.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/grewilttb.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gqcwirzxw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/ghijcsvzw.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gggpkhewd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gxgweuvxr.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/grrhzqbho.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gnekvtmim.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/guwyetbod.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gvfjzqfol.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gjbmubrce.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/grsywjviu.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gpzghfylg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gxidcpryu.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gynjqxnyc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gxysqpwcr.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gfmhyxbsp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gjehlgvni.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gimcnqsqe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gaxoxzcpk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwjzkhktl.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/guatgquri.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gofusjvzh.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/glugzqztm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gljxtucmj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gdvlzvois.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/ggnclopzm.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gloxcubpw.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gcfooberu.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gemuljdns.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gyrymosav.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gildlvmvd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gjanebiqz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gvzszssgn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gpdphmfkg.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/guhnetzyh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gbyqqfoky.sHtML


<!-- 参考信息 -->