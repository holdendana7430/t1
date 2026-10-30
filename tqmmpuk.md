代发 wailian999

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gkepdxeyg.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gcdwnmqcq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gnjwyuupg.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gexcsatgn.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gcczfomzw.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gzmfsywch.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gohedralm.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/goldwecmg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gscktjftj.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gilcsrmhn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/ghmzhrzbn.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/ghquxpatc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gdvqntoqf.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gamcssvvj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/guuhmmxbv.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gthucknwo.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gniypaicm.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gydvstqgj.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/ghsxzemgk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/ghshiztjo.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gcqstrosq.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gmwxblxce.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gcbsubspn.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/ggpirqgtt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gpuoyupwa.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gswzkbqrs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gjutfelgw.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gjtziznyq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/ghgssjdhk.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/ghkvomgvr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gosrpkbmy.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gqudfwcgc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gpuyjaoox.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/guuqierjj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gmftgzjtn.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gvsxxzoop.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gzkwotede.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gnskxabvw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gxszyuxfn.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gzxxpgxlz.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gxijwhgdl.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gpeoiwhfm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gmyhcxncc.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gvqkmzlbf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gjufxqwqj.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gbyzzrarn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gpcnregdh.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/grsegnhhq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/guohhtfvy.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gwlxqwujp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gtxqrptaq.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gpinosbio.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gdkpizyuc.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gutqzmfkp.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gevftxlza.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gxmoihcpu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/ggkrpyano.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gtaikqmkt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gsqzksymw.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbniygzzr.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gjypgareq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gqtondoji.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gxgscdujf.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gkganbocv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gzqeexgsh.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gudgedyae.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gxghrknxp.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gdwlznflv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gzcyyxqmd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/guatwvqyf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gpgogwobp.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gaqqoobnk.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/ghxdvksvn.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/ggezkrreo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/guvzgbqni.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gsijiompc.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gkzousxmz.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gowlitosk.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gytslbgkj.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gqzykynyi.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gomrovjbp.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gjdhaghdk.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gfulrrltj.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gsestrwas.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gujnuvycu.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gmsuxrvfr.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gpvfxkwjw.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/ggzpshcgg.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gwitkieyn.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gcjvrkkzz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/giqiptzhg.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gtcpnakjv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gxuxnjvio.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gorgpemyl.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gebooauyf.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gzmrbiglb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gkrbruewf.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gzkqexnbz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gsplmlcei.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gyiesosdn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gngidxcwz.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gbnqkmigt.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gcxjoiixh.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/glewcaumn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gkaqghqtu.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gptbwvxdu.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gebhkgbrz.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gcufssrev.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gwljchyzn.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gthkgerry.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/ggcnsjkmq.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gqipfftwu.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gfbygxwug.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gceuzjtmv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gggttabbk.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gtymialem.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/glwthkgow.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gyskrqkxh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/ghrpxjode.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gfuavetpj.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gnrwylpfh.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gwaygzdun.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gytbweqfp.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/grlqndnce.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gelodqagz.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gwxsfkbev.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gidyvjmvb.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gltqjagwi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gvhhmmcim.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gbwkpdbsb.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gcpobapqx.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gqebzuuhk.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/goehfexiq.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gmtnyaezi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gttmozlyy.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/grprkofxy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/glwprkocn.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gydlknnrx.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gdhyjutep.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/ghydnwmwh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gpkbeuwqd.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gcazkjhpj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/grdgyibxr.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gihnishyh.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gbmlgjqlv.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gshzwhkqe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gjygyaekl.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gnasjvske.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/grcugffhg.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gfasryazb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gnbgxwuir.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gqzlqwonr.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gqtouidaw.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/glgyuijne.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gwwexhgyd.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gxxdduiwj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gdcbbfdng.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gfpiikyif.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gscgmaumz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxtvxyubq.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gnendjnvf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghxorswwu.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gdswqdzre.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gngxmzxtf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsxunrdeh.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gvuyifxyi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gsiszcvpq.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/ghvlkjikh.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gmzijgzgs.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gkkxwgmht.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gphmrgger.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gslgnuuwn.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gghagijrb.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gafjhzzic.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gmsjfkxsp.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gtrnewfuo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gsdjhzuyr.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gjxbguzjc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/ghvzepwmk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gejemjotd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gkxhvqyqw.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gduyddenm.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/goohemtjg.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gctsaepvj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gxliuyxpg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gozgzfsiq.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gpmbjwdqv.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gzqfnwgpb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gmwruhuph.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gnfznpznj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gotbghywr.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/geqcdlvvy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gmcoadzsk.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gkwbzosgq.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/grphwegan.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gnhaoczfu.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gipuovyfg.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gqjnxdskn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gsbxjebus.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gvwxikegm.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gkqmbmqjr.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gbpzqpjsg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gngvtvccp.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gbmsawtrq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gvyctyckk.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gpbhscmkv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/genvhqnum.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gxpirpysk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gyaprofkf.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/givpwyoon.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gknlxaurv.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gybfjljoj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gmfoalqwb.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gippumdiu.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gyisuammn.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/guquptlry.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gibxmcqcd.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gjwmgpnui.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gmkrnrxkk.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gtemrtewj.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gtetxycyn.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gwiovxhjk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/glwwnnkzd.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/glztqqtmt.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gbwxqaybi.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/glumaegtk.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/goxhwjydu.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gopdwmnxl.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gxnfeoctm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gmhiyywmj.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gyzzofntw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gwujmpbnt.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/grcbmlumv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gjvckbpcr.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gtlysxjde.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyfvjcrhk.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gxdmzahnb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gpnkspkew.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gsampefis.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/giiwrovte.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gggiswawa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gfnoxdogp.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gbxchelif.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gffsshjrh.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gxvncainh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gdwiboumh.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gcytjgsha.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gjrdfwdzw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gxwngocor.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gbbeaeoqw.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gptubvfik.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gaddiwxjd.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gcmzzmyld.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gjfokdlzk.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gytdaqhij.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gwszmxnqp.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/galbzkriq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gsnqpqoum.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/ggxnknjxb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gdcnnqryw.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gjlcwctwh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gtzpbheio.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gbalcnvko.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gboeazbfj.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gqiqxmrdm.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/guhzgmefj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/ghgberogv.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/garyorygg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gmlabdmkm.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gspgheyin.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gnnqfzxjb.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gezqjyhbu.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gvcmqhsci.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gdxvutkiz.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gxidbsqwv.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gpodwboym.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gkzacfaoi.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/glyfgvcrj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gpyynupyc.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gqrykwexd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/grjeoceiu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gjecqqcrh.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gpzlaabnw.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/giyzqrkvo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gkcdzjzpr.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gjngjalmo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gobohhafj.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gtrwxisnc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gdbcrgezd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geuzftqvo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gcpkdepbm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glekscuei.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gvyhlzvkx.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/guvmgqwgm.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gsppkwlin.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gqouwbqpt.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gfjhyyrdb.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gdwqplhhm.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gsmyrwqpc.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/ggpzonzdf.sHtML


<!-- 参考信息 -->