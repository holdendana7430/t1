代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gnpwlbees.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gzzsxiwwe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ghapwhqsr.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbjeqgnl.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gxlyzvrae.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsljzumk.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gkedxnvjj.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/goyaiymwv.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gusgzrrxp.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzkvjpzfi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gscwpsblj.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gfdnehyjk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glksrfxto.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlmygzne.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfcsglev.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guhqfcoix.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxjbtbuo.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyendzlv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjwakebr.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gekexktiy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsbdywcid.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gioxoaipa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glaciwfiv.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdouhpcvo.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gztycycyc.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqldbnge.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/guspdjuij.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/giqsdntmg.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gukveimnq.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gsynwxxwa.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/guxgtwfoz.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzmvxznz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmwedfljr.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gtrtjgtps.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gflqyfkyq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqonacghc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsudswyjv.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfaskfmr.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gdeogxhxb.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/guzpkznmc.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gptqcqvbs.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmqlumvd.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gabtngvao.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyblxobz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtxndqgm.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwqxzlhr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gextmufgo.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqmrxiito.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxrgfrvjk.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gjzudzpjs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginbyjwwo.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gdgjfczsv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzvmhene.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gwqlsvtzk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gewrwqfta.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/ghujhnnyu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzkrhxay.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzshwmlm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/giuxylvcp.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfxieqod.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvhvfspg.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gspnqtakl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/ggadlfumt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvazsayb.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/guhjxqavd.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gpwtklrsv.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzxwynqv.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmjltxju.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gkwcnrznm.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcwslwxj.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gicnijald.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgokbwew.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gbmgwlatz.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gepgdhtmp.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwpkhleu.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gyyplyohv.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlhbhqrd.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwlukhvg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjoumhap.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gjcdjfjnx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggxygyoqc.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwfexdid.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcejgrgnu.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpgauuaj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/giavoglqv.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoysjrdu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gitrilefr.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gueqroxjj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gjaqbdcru.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gglxcmobf.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gusgdmvff.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnwrbwbr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuhsrynn.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giilsdqsp.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjxgwyve.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gihwyseip.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnukdfkd.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gozysgmjl.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/grleheage.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/grsvxpnkv.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gshwezvqn.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gegpmlxlk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqndplnq.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwqyxncr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gveufokqc.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzacdokr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclryofdg.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpuikduh.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gvxdzanqs.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/grzpjwgin.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gzdrtvhnt.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gsfmpmppp.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/ghdbppixb.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gfnulqyzf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gwdnijbvc.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxsziopq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gelbweqiw.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gyoscsgur.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdmooegy.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweavmvuf.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhvuvmeg.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqffnuiqs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glekvliwp.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gfigjifpc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlcqytzt.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/grlndjsbd.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/geqkfmzym.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gpixvheoj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gqswwblkz.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gwubksrtp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtlgritc.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjpluobt.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/ghpcfzthl.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcenmjuc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/goekaoymt.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrgiwvxk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdkfhuzj.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkqsscty.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gzlscyrtx.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgitrfjb.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/ghmmkhgzk.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgkxuxjx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkdmmigra.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrddihds.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqvygjoc.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgerrvyy.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gpcgitsfs.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gswqtorfq.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gnnxtpqph.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/givxhfmgc.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gxannnlpl.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/grlaivpby.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghnnqmlqd.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/giudduwog.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gqherkxvh.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfbzxwgi.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gntgbxhpl.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gmodjbrah.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gfdcmzdco.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwydaxsz.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ggxduezwv.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtdvcjor.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskbqwkkt.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gzdswjgcf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gnrrknrix.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gawcnsgue.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gkjjubara.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gvimafamg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gcrgqxnmu.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gfaptchxa.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjhyupen.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqjnjyzh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/garmglqwv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyuopefh.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/goainemiq.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjjynvjie.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhlqmagh.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/ggbclampu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrxrzkyb.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gghhnnnze.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/grapgkdrl.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gpflsgsbv.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbikjdgz.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gekkdrybm.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gganlxkus.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghudzerpp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gprtcommk.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuqdwrvg.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gskkeobcd.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdiektqw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpohdvsrw.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gfghlwzsw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gedvyqofs.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gcadaynuk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcaojtwt.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqdwdiug.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gzcaotkop.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyccniedj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghybvaryj.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gsapisgof.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gzedbyaxa.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmakuqyx.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghoyinsjp.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gygeqgyhq.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnbfyqcx.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhhhbjku.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gqmsehftc.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjqcixikj.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gnahrezot.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkgtrjph.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/grqcxmmdq.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/grkvjuemf.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gdoxxwuxi.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpezqrmms.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpjtumlw.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoraadlh.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/glznxhrwf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjltwxcck.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gozblicka.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gishspkpi.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtdqzotq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gsrzsfhbq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdehormdc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gluzzwgqg.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqowwpdu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmrsrsgr.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gwbizpkxa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrvltmwk.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gyfeefxzv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuvahjov.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopwettye.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkewoaldz.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqschtwqh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gbekzgefi.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gagzxwoyk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkooquyk.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnkeitxzy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgfryioz.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/galayxllm.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/grcyzbzhh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdffrzrg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpopmyyp.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gcibgvkja.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuqzkjxk.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuvnzhtv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/glkjrcqoz.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gyabykeqc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glxowtufo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geankszvr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gehquhmgl.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggeuiyrgs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/geyqujtdz.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gjmhfkyne.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmkdoijn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gqrpaeoyn.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gzyruacwd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/glqvbkxei.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfafnvmwe.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/giqyhjpzg.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gqfrwepwi.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgbsszrv.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glefbtpez.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgohrrxa.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gjcbfxoaa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnaxbebc.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/ghggxskvt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/glfmtdjht.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gqpdmfenm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqtyrwpw.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gwujanfsn.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/grrivkrwy.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpdgaqak.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gzeeqmanc.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupvirdpf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gdzjldtod.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gxphcysmh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnxbfrsh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gimgqwiug.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gqchmwtgv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhblcdbf.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdiqozpv.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfokoddi.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmvxgvxsm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwfkrqrz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gtwbksqdx.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gcaloqswm.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gttjpqsjx.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoolsvgh.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ggoqtgkbh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gjanedvqk.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gwctkezhx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gziibiyxc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisriungm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gqhsehono.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gypqtlcvg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucdmgtcb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuhiawss.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchyrcgch.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gdcnqhnfl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltildpsa.sHtML


<!-- 参考信息 -->