代发 wailian999

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gehlxbqrx.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gbzrbdwna.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/getgbiheu.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyqynvsc.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gjqpocqua.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyokbuums.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbacsxpav.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gowdmwmxy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/glhomcekn.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gvihalvtn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gborcfcxt.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqziwahc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnebiimey.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gkqthfgzq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtihuedxo.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gywkofuhb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaufnbmy.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gyukvunon.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwiglggb.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdoqcyhfy.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glukiwisf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/grldycbjf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbsbribo.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnlkapnv.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gofzyvhmw.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gsudqznmg.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkogumesp.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/guogczyny.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmwymoqos.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpkziifd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gthtyixbt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghulhkyeh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkgcseyh.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgolkksq.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/glpnqvzil.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gvokfziip.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gqpturafs.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/giezjvbch.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gejatqont.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhdxznhg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gakxrjiyy.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnzghemu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyegztwt.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvtxhgtn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcskgpwi.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/geovrxqyg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmefcdla.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsbjgupk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmwjttao.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gfviifyyb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqaouexr.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gbhtvgkgs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjrqtpyn.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gixnibjcz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gscmzpyqp.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gliymjhob.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/geekdzrep.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvwjrsos.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrvjufec.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gftejpmgp.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzfetbok.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlnkzhas.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoeyxbom.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gvshzftbv.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gzpjcyqnm.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gevekifvr.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxtornqp.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkkmabvl.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxeljfqd.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxelankpt.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmunipys.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacavitha.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzpxmeou.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gbctcwbuh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/ggvhyrpca.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxesrzplh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmgwnasi.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssqperpz.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfudfbpue.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/ggyhflqyw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzgjgumm.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gvahaqgal.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbthwjubr.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gztpbmmrh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajosxjwp.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfxgeyak.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpjmretb.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gcdmvpjdu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gffuzzjeq.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gduvalvaz.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwrardgx.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gocusivgy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdrnpkqg.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzkoxmvd.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gfdioidui.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gebihekby.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gdexmagur.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glijfwday.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gtooqwjyq.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmyxgogr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gahjzfohq.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnanvdnx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gizstoywy.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeekpsgf.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gnizsjcgw.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/glltbjhfq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlccfwem.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gztmmdrsh.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gkrrbwwkj.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gpkwxqwxh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gvkylkhvx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyabbnjwu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchfiftsa.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gcxzrccwa.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfksdiqf.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpqsbdwp.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gytexcsvy.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gcxrrtazw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gukfjlsai.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gxxcbdsez.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwyxxaxl.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gnzfggfuy.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gjcyzcpym.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gtywumfqx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gpwhbzjla.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gcqabvvei.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtlyxmknp.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsimsofbs.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/glfxjcjta.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gyvtxkgnz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwkpshxs.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgichxyd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gfchonzel.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grhdqwfuo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/guwmwudat.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gzztblawk.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmblinyb.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazpipabr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdekkihhs.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gkzkcbtsx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsohgttl.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gyiqfdngd.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkpgvuef.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcnvecbly.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpefqufvn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbwvnooap.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxuxhxnc.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gqymkdemm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqzjrmefi.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxrtngsg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gdpvsreqk.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/ganfktwps.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/ghqyvlynf.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gmwnrmlkw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gspaxspik.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjrbukit.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gxbdtzazg.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gdukandts.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/grqznpkxz.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjgkgwyu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gztifiurn.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gtmcmsinz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrhjttsh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbjgtwsg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosgiyygt.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gggvczgsz.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtynyhcxy.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gilxtrsbe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrabghqv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gsxrrestf.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcrmemjf.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gflboxmrx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqjksrrw.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjajqnym.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcotdsno.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnxgpxfc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrogohse.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/glvjazfbg.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gsminkedh.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gpcmrzplw.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejppfwao.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnolngxbw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbenfccmh.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmtjsukt.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvyqucdv.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/glbefssrz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqqqpzfl.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gxrftmauf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjulrvyrm.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gyetqhoew.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsvqptze.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvrlmxiu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruxdrkcu.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwwbgpbb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gqzknxpbm.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gfugkezdq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gcnymfyrg.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gnghjfvey.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgvpdrjc.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gnhlhzqly.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gatblmufl.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpjbrsjr.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gboodthye.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxkpaegn.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmshydksm.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzkmevfmt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gjujnyhbz.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/ghbjycmbc.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnhsvlka.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gexzqiycx.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhnxjdhq.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gkqasvofk.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gqvixrbvm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gysvdeylg.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gorwwgedn.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmpwzxxc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxlnguzg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwpiiodn.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmkaluut.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdbimgixu.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwesgkta.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzscsgocn.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gxobkizge.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gccyydtwt.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gsqlygues.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gvkadzath.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gvirkcvzj.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/grtotqrdj.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gekodxodn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbwwvgrc.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhgqzgss.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsraxvenm.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaztqtbna.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gwhkqdxsq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaetovhg.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gaydgrrjb.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gtoepqaro.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gubtmcftr.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gwartwmhm.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gidsszzpz.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjlnftts.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/grjchbxzd.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/guwdpygbf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcrevhcwg.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkeenkno.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmullmksx.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbwzozxg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gmkukabnl.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gibitzgmc.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gckyzcbsh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtcgpjzm.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gzgkudoxi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gokhfaneh.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/grvuerwma.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/glquftrtq.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gsmecuguh.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbarqblyp.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gdpghpeta.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gifrncprk.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmwwylce.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqctyzznd.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/guatsdhrx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfisodwk.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gmgjionfq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlrbcbdn.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/guclzvgvt.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gjdfknbyi.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gixjdoyby.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/ggjxxrtaj.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/glayvdnpz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdksddovf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnkjfheb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/guukieash.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gixdjlnkw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqudddbe.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfqwuhsh.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gdawytwup.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggziavzff.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrwekppr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gvusdwmje.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyapxnje.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gbjjmfgef.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxotmwfoi.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehlbhxfn.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gwsshkqzx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gjvswxmgf.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gicuyffrl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gezhmclri.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiswswje.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiugkrwf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gabvqxpyc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzxiitmt.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/golehecme.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrynchji.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqgoblgr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gkiigfhkn.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gguwiavcy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmisjbjlg.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gclquzgtm.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqqxiewf.sHtML


<!-- 参考信息 -->