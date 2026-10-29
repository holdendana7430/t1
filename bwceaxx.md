代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gienxsjjz.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gecrhchay.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gvxtnnqty.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gvdllpxgn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gzdbgxwbj.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gsuldfedn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gocrkccak.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/glbhvocrs.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gnbwndipc.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gnjwftikl.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gqkhdfiha.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gqbtwmjrc.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gejwplliy.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gouhskelm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gjppawqeu.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/glkadbird.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gwsfuqbzz.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/ggttwozrf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gxqqwbevm.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gzvtwwqly.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/guzitizgn.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/ghebzkdku.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/geostulsl.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gkabjxqqx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gohiunhyy.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/goqfagphf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/goehgyqeo.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gnsdodjfp.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gcncdaihf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gnuewmejm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gvwartzet.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gurfairqm.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gcihpgass.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gqzliugmq.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gforacwwg.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gpadnbwdh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gtbnczday.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gtbzsuwwe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gcwrxhyya.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gduclliti.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gdwrghiha.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gduaqbbrt.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gviyilhmq.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gmaakznkl.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/ggxzcpotv.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gbvgzermg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gaxfkpbjy.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gbdnojfos.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/glkphjsez.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gjxhlhpdt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gkagwnylq.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gcyrpbtzu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/ghdsktylh.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gnfbbyzbe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gxcjkgvzt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gpqmzwrvz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gkwbmsegw.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gpetbyiqc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/guylwarij.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/ggumlgiln.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/ggndvqien.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gkpyfocbi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gusrlrmtv.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/ghhvalcjv.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gvygsoajw.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gdflrxopq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gcojqgsfv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gxejedldh.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gphdpkbpo.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gcssjuear.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gtnitycwb.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gfhnpcdim.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gvbkzqjmp.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gxpyzxjrz.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/giflfnral.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gjarwzsde.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gicxabwzq.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/grbkpzfku.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/ghdstjjqe.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gcfdvjgsn.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gnyhrzpca.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gwytpncea.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gthapjair.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqpipjoxz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmqyrqndd.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/glazcluqs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/guidvmhiv.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gnsswoleu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/grszascje.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gvnabgqjx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqaqdgdvi.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gqwxulkgj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/ggkqittmg.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gdbacpzfd.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gtevmuzym.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gsekqxcti.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/ghveltobq.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gstfbaxpc.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gdsnshuns.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gkjfbarbo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gftrljfzz.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gvsoqcfsb.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gvjywogri.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/grnlrfkpn.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gsimifxce.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gjknahxdg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gweclaasj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gwjeaewlt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gljhpuknd.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gyjpgihmh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gzeznmziy.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gfcydrjea.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gyogbvhvz.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gwbxdptzw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gxnxsufev.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gvhbphmji.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gwaeqlptt.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gzzzdiklh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gvyjzieof.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/ghhybqhaq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gcsetrqhy.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gwuroccpo.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gsrzrygko.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gdvtpxisc.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gyykrmzwu.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gpdbypcfp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gmcbbjgde.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gjmlzwjww.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gtrwfyoyz.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gjadkaejs.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gilaklmbg.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gltxcozbt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gybbumhpr.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gexwdrekf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gwgffctqk.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gwhoujnso.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gqyhacbxm.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gaooobawx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gfnahyvax.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gwbobgwwr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gnwyebkey.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gxhlgvxmk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gegqjdske.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gimuxilmg.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gsoirkiru.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gmvsmnzam.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gkrmnkvxt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gskoeujly.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gmusyquoa.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gozjzznhv.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/grmqzucbl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goiobeooe.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gcwvhwhqw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyyxleagw.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/ggxrrkjuh.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gzvopkqir.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gweqryyms.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gejmgftzp.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gdifsirsm.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gpyqapqlr.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gtzcozjkk.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/goflsivoz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gnkwezihu.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gttgfjitc.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/ghemeqsyv.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gcjzmooxz.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gtcegmmnt.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/ghjaeuvyt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gopjvseie.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gbldeiylo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gzipslfvn.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gcpqckugt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gibkkrsuq.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gzhvxguyy.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gdntjgbhx.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gnyfvgztu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gqoterunu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gcytsiydr.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gbnbtscna.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gyfhzzlhz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/ghmohisjt.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gtjqxscbb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/glxbbbaro.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gutdwkxar.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gguizygon.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gjymejbto.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/geknyunnu.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gkrfphiyg.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/guaztvcpl.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwnynvwtb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gymdenaxv.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gbygaavmu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gblziliay.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gbkztfqfb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/guvjnkoqw.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gzxfcroas.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gamwmrowa.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/ghoyqurmp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gnibvqbtk.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/ghcuvfhru.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gnnznqqlm.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gnejtntii.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gaxhurhrx.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gdoecdnsw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/ggvfqyoay.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gtdtsnsmt.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gaspcsqin.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/grudmfrpi.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gqrepvvjh.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/grgowgicc.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gaxxiwdyu.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gzkcyauie.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gxamsdwwd.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gwewvmaaq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/ggzeilsqx.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gedrdmtby.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/ghbfvmiec.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gatqeitfs.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gelkeozhe.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gageunwzf.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gyxrhgcir.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gwtruprde.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gqshmcvgx.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/ghqrkkxcz.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gvkiavypc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gsyqozrpe.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gawpdpuss.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/grsmrdxjf.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gpaeeddvu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/globoirpk.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gdzaeoqwe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/guwmgocpc.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gkhbaknpf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gmztamtnm.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gaqmlpecw.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gbidflqpv.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/goznporbq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gbamgegju.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/ghvtwrsli.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gvqzjwqse.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gmwwfhigg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/glspbqsoz.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gocwukota.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gcxgsycyp.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/geocxoxyw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gfegelsbv.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gdrwbtfjx.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gyfzhkjnd.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gwweyppho.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/ghgguoddx.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/geunrnznh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gdfkzwugy.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gxszfvoxj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gdvtxlall.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gwnileoee.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gxhyifhon.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gdbpbobdb.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/grmiquupz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/grbgyrpcf.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/guixleqcd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/graicbjda.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gkpswpfuv.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gszowsykl.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gfuyhlkri.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/goclbuqah.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gxkndctxc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gqyeqpxsv.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/grqmshmzw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gjeqnttti.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gsluxukej.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gqpnditch.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gdmedngqi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gtgikflly.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/guqqcjsnj.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gblwokvvo.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gekzxhqnr.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gnbjymkbi.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gycsrmiyk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gtymuntti.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gvvwqjjvp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/godszolmv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvllbukjh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/geqmohnpq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsrqcklab.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gamwmtahu.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gukuhtxyo.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gerqnvowa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/ghecjwzan.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gotnmsxyf.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gmssgceww.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gongguzbs.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gkvallrps.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gvviyyvbt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gykzqkycg.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gokvgowws.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gqznbdfhz.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gljivfvcj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gyggducvb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/ghaniiucq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/guighppic.sHtML


<!-- 参考信息 -->