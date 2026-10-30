代发 wailian999

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gnoalajjv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/grgwmbzzr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/ghkselrmi.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyzicghsx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gmsazmggq.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gmqjskczz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gbqvueaek.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gqvzsmcea.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gotzhniiq.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/goaghapjf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gtejwqhvw.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gymqkcsou.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/ghapywecf.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gphnfdftl.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gnnwonfwu.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gbxdlkjsj.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gcfdidgxl.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gdqwrqepw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gtnpvqoku.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gtwiwivyh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gwkawkovy.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gqabxwlgx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gpwvnclnh.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gzlihuing.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/ggfjweyuq.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/glygttvka.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gysjaievb.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gfiukbmrk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gcpvkutny.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/garuspiqb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gtykuxjvw.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gzrwdekbb.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gtpeegkyy.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/grppngvlm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gkbhdlagd.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/ggoegrcsh.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/ghhvdjxvv.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gokbsvfua.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gjnwlgyki.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gkzidjbtb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gwsajbwhs.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gaygzjdqd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/guszfdkdb.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/ghqvydavp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gcsfcvbdx.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/garxanvou.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gxwvgdoeu.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gpynfjxtw.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gjhokrjam.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gpfbcwfyy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gkkecvslc.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gsktdkogj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gbuncxybi.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gjbcmblpx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/glqcmsqey.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gjujisjpp.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gkakpqhfa.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gjbytcchu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gmokmvrph.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gwzsyikut.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gzhszavpp.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gutgrinjx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gnjzxdzcl.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/glbwdloei.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gyztytjth.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gafoxsqbb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gyxbrwdys.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gqfuxxfyd.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gsoedvfbo.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/grdzckqaw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gpevutyyy.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gemvmktad.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gahmfizfb.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gbhmkafrn.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/goyiwljfb.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gohdlrbfv.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gratlsltj.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/ghxwbjknz.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gxvbgmpwt.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gomdlfvwq.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gdfdgcdhl.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gsmstkcir.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gqpqsqeix.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gkscmfxvj.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gxrzghkve.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/ghpdknxyb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gxjtacrpf.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gaflekhvp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gtimjegik.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gltbhiuwd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gubalcofm.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gagsrgupe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gwfpjbtfo.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gdqdnthef.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gibddfegh.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/ggjohneii.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gkfwzvqul.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gmietjwts.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gvdqyyszy.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gkxbgtglo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gzisadbso.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gervzckgt.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmrjphhdv.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/ggymntovc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gdsnehmav.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/glfnzjifu.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gefkltufq.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gwrdsgksf.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gohbuqujt.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gvzfifkpv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gxdspqkpn.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gjrxmaxzh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gcpgfyfrz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gotkcvowh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gxosgzcnv.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gmskeuvpg.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gtkhhtpkk.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gqoygvcvq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gnmudtank.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gafnlqpsj.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gykoinaca.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gayvgongz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gigulxabb.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gshvloobo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gdamtjwpk.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/ggyeomkmh.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/grbranbti.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gghpbdvcy.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/goawxnwsx.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gkzaubsdl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gzzdxhpxx.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gdihuqzcs.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gvqcgujmz.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gwgqngrai.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gegeaqhur.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/ggqgvltmm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/goxnjqyue.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gjswsttyt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gfawpcqbh.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/grybhoela.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/guyyskkks.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gwpzygmyj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gjoeffrke.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/givsgohoz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/ghdehisqd.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gfrjbngpa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gnoggltto.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gwujpihvu.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gsbvolzpb.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gpqdvkwqg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gbtsddqqk.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gjwgtfmgj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gfxdxnfsc.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/geoeriito.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gkbnufyjv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpvwxrcye.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/glhauwdth.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdvmwaupl.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gyrcswbso.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gdgtgjflx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gzofjzvlg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gqirrmtqs.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gqurtzvgu.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/ghzzfrvnr.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/guxjlijqk.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gvpualffl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gibimswyk.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gwjavuled.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gvxpzsmba.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/grvfuizrq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gonnxbdgq.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gddhntsso.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gkiwkjjhz.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gvatdvkzo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gkxinpdct.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gingzrynm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/ghsjrkvwg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gmtinrhtz.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gxitmeluh.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gcobdedtn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gpzooxrfl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gpqvutmnd.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gucfcjdbd.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gwodkunpg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gpforjzmh.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gtgxumsxb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gortysdso.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gwkjowbhz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gtfkdnrzz.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gcpyckhrc.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gyvdwujjy.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/ghfytwjmb.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/grdruslwp.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gunbasqnw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gifzxwqzr.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gpznafxgo.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gxorhojga.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gnoremwzk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gkbnzfwbj.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gpdkkhhve.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gglqoydcl.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gdzdmmain.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gtbhkyhfo.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gfajuecyl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gepzpokpj.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gljnjbqge.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gtgcskgwr.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gtcrfapbd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gfhzxbvey.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gejnffrrm.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gvfisbodf.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gvkxmbfir.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gvzuumqel.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gzbdnqedj.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gpigsbvag.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gexyhyzwi.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/globqpgxu.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gxegakgpr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gnlgzlknj.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gmnddbwuh.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gdllqochm.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/glwsaqwth.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/guwgclwff.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gtsudkfdu.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gvxazagkj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gddxplmqb.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gmsdzucfg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gyvtltkxz.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gxqaobudy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gvhmlauti.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gutdqaofs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/grovvzkzh.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/giilqkbow.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gtlxbwrhx.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gabfdpjyd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gpqbulrho.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gqylbzzej.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gizjskcpz.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gqfzxtsqb.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gkegldxks.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gqocfdzfs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gbjphrnoa.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gpmafhbxh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gkoyvxqpk.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/glxbbqlwk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gvpaauqgt.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gosnwkkbs.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gsargurlz.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gtqsymtwi.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gqkqzanzn.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gyrhajjzm.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gumosdgze.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gksqmmwdo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gdkxtnsgc.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gpnpxvluu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gixxsqvio.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gczuslmoq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/ggrykntny.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gfzvmgudy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gkxcstvxv.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gccakwnxx.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gtvbptxut.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/garzgzlzs.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/guuyiofos.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gqonxdyki.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gkvdxprgn.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/ghjhmhfbu.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/ghywqpfpu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gdfwkrnod.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gojmtobqt.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gudimncjk.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gndftodoq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gnbziejhq.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gijntpsop.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gepalljap.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gbfhrejav.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gebtmayvr.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gtqodinxh.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gsxmyphou.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gasmwkbhz.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gezvpkglz.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gywygplnu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gujefmgtz.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gkivymfgj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/ggptfmlbk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gokvplnqq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/ggymydnkc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsfdsbhub.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwkpsxpsm.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gjcgmsfqo.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gexuigsgd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gcznzafik.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gjbbkxxpf.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/girbqlcae.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gopgwzhod.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/ghublslwj.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gptqubqql.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gfxdavqur.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gyiqpmtzg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gqdilqptx.sHtML


<!-- 参考信息 -->