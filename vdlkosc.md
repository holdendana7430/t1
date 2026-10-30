代发 wailian999

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gnwrxxrak.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gxqsvglwk.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/grllmyiia.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gzlzipeur.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/grrvdohzo.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gksvaspjr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtipezpgp.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gbhjolooz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzulyvizm.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/grdskjtnm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghaupvgyh.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdpfqixrj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjymmguo.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgkdspbh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpuxagja.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmroufxzo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwytteand.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gostktjjd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmcylukz.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtctysgaa.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gekunulbs.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimnnkhnz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gletjewjv.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gznledeef.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfcindav.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gfpeoagei.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnyypzkb.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gruybtxrn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geurrxbrx.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gocgxvvfw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwendzkuk.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gymcxzsxy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwjshcnoq.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkcdukjr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogsrxfmk.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gpkjjbkzn.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gmpokxnzx.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gdxntgwzy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gresabnuy.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgjwyobu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwrugsqjo.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gilptsbtg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gxejxnzuv.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkwluoflb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpofkcyva.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcqttdcd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfeazsexl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gnndifgol.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gzpczdxff.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/goprzngpa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gavrtyoif.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gyifothal.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gugtkfxta.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gvpffkpyh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfvtpuck.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnzgcxsj.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwhigipo.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gvoxzdhfh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/giwglbbac.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gksauawrm.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiedcvpz.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/grwnoolzw.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gmctqehsl.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gtiepqqoy.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gqdzncruj.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpteethrw.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasfluyyy.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiwqpjxz.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/goevdegsb.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gegvvbiod.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnxvuvoi.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gbvrvriza.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gzhjfukso.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgxsvvvn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gatiazmrg.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvegyvnux.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzavrqtiy.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/geejyccdw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gycdgutii.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glwaszasm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gbttfbrmy.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gbviqlagk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gickidzvx.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfuhpvgw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gdwrcvldj.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gogjzxbfu.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdkqbymgc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqzmvygc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfqepsvm.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gikganjab.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzepmyddn.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gbdwakelm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gpudusslt.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdrlkwity.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gebejvrqt.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gftqbulhc.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqqqktxo.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gloujzxtb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gtlwsqwhs.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/geadfkmqa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwlhagvy.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gfiuwaizw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gxsowayzg.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gkrvrfjhf.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlmxxkzv.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwsnjnyn.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gjfptbezo.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gtdqumque.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gjropcsvx.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/grjzynxhu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gasgthlqj.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gctdrsmvh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiygxpqj.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gznaqykkt.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrwmbvgf.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gyihnnhtx.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/germpixco.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/glfklmiod.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotazqlpw.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gxpbvzfjw.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gfcnpfsom.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/golybjnsy.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gedrckjgm.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvnnoisp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gtlnsxxsz.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvzefjba.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govdjyysr.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gspozbncs.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipxphvoq.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gzbxbeiaj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guokpedih.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtsotxry.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/grwijhzdo.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmwvugid.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpkoxvth.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gdazaogdw.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gvzrpyxwr.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/galhhvvtk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/giswxfirp.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gvakehdfx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggqzntxfs.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gbtdoawwy.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/glueoovgg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkplpvrmk.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiakywfg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gicndmhzc.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvhzzqte.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gbextaozf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdbbxjwrx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrsbwsim.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gzgximqig.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gktxwytzz.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gefxwqzty.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gcljewntl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/goitelnpy.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gsuclpkph.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvfqlseg.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkppbmuot.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gqlryoyae.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcnqdrza.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmupcfwg.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gwvjztxws.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzqkldpt.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/ggzmpmfjm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gqldxbjpk.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gxuqtnime.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpznnhsq.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjqkhcwv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzxyvmpb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gqwplsrhm.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/govnikivw.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcowzqtu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaoziitb.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlyqjpia.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiydijle.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/giwkbmldk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/glcnssfbz.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/grisddxkr.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcpvovlv.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gxznmnfju.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmuojwaz.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqaanbzx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/guhyavhxq.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gerdubmmw.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhmdienr.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/giakltbbk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwsurbob.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwzdcfne.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvycixivd.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gcxajknyl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfqpqnya.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gorjvwmhp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjxwwkmu.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gffwzpfvc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrmayuev.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbajcvqm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/glggyjlwo.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwngltev.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gebsebodd.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gqyehfhdm.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmsmzxue.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswjfcpbe.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gttzibgze.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsrtqujjz.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvnakbmr.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyuapesh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gyxvenxhs.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gljxswewo.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcgicbyq.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkbbjlha.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqbwvryh.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/giqccrden.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/guhjoqcnw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitmhdwtv.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzcqevee.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/guzexxttj.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gdefdmmii.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghgijwemw.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/goziwswcn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzkqggli.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/giwqbmvbz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjywnheys.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gvuxsqykj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glfpooanv.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbgalvid.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrhnwlqr.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaqwbnja.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcrgeriz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/guiytpqsz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gisozgnun.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/guciwaboj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gusvvaprc.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslpqktnu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrsgjyqf.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/girfphmlh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gimuyasyf.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/guqyvbthm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvcprebv.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdecrqcj.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpzpuaev.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/guomxpcsz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gfaefriay.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvblhkwf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtnpdtuty.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtsqavev.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqfdmyhl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwgtshgf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gopkrgyqb.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gahnchsxz.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guudiznfs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuouqshn.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/ghmrymibx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjrnjwxj.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjgkxfzl.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/geoshzlbv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/grlrqacsu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gilshpxzl.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/giyksbtfz.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gvdndmqxn.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gokmumskr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfocosxbv.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gzerflixd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gmnuyeozy.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gfmlctvad.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsonpfykl.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gpffbivdb.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gfgxduxwv.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gmdfsuetj.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gnuwvbdru.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/guipkrldd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhplyneg.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gjjczhbsq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/ghdjqohhn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyosbyfn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiomksxr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzhngjkca.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsumzqvil.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gegmfrvpq.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gispqwmab.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gjkthldiu.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gvspdpewr.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gkiilpsve.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gijfdyqnj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gctbesunh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqmbwxqe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gvuwluezb.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/geldcdvkz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/glkhxgbct.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gincysvwc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gpunvtase.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/goqdoyavx.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdnlcdus.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhxmoxym.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gmlhpfzpo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvsdnsgu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsexaekh.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gkdyjmxkj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpckeqmqo.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gvjbwyjix.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfircsqi.sHtML


<!-- 参考信息 -->