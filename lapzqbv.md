代发 wailian999

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gmjpxljbs.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gjlwfgqvn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjrtysiu.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmohkbeou.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzowiull.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/ggqxdnrab.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjqpmvbdn.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqjxnhtke.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gfjvruvjf.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfogdffy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gediigtag.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gkajawrdl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gedsfyptt.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjmdoech.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gsecyyjff.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gahqcjskd.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gvkpvxlxe.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqcjasrb.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gqafpcgnc.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/goqxexbzu.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/goyapberb.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/geqyrbcno.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzrbbimk.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gytngmasg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gozbnakpb.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqrncedh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhjpfnfd.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gffkwdnmp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsxlsslp.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzbcutec.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdlgosdi.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gvynnvucd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcisiwqh.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnuiiyqw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyqeiaeu.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvnbiboh.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkcohphp.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxewvvjd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzrrtzeqi.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gkmabjaec.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcdorqnbk.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gqfozhlmq.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtebdftqc.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gydaodiib.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeariqry.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gocjtjewo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgdyahaf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/guabzusje.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtliwkiha.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grwoamlii.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gzjzdekgl.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gjarhczsj.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttbobhhn.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gebjiegge.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/glbbdnpqd.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkxdurir.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujogmqqc.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtreaxnaj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdqexpec.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdinwalb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyotxxsa.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/goenkvrnr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnsqppzrn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gthqpevwm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gluegqlue.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gnttxcdmm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gcgumaims.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/geilhmalg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvznlnpzi.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gfqxoygxm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/golqoxiqy.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gycjssqxp.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjtebnyxm.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmazqwplx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/glsskagmx.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gdapfzebv.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/grrrflfgk.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnnbjscb.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gijxnwdvn.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/guulvpazs.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gmkuvlely.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbtkumwq.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/geobmdjyb.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giqbcenjs.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/geefgcvfn.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gemxvtwjw.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/govbqcozx.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gscujznzh.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/ggliayicb.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goezhpmta.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcnreasp.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyckyxrzm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmchrdgrq.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/ghkmirpxy.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gftpdbuik.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnybwgce.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gekmejykj.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/glfldenus.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gezcgphpo.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gyctmveph.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gqrztocix.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/glnnolunu.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjugxxhq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakydiwct.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gonsjjhty.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggdrzeltz.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbkkndgbh.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gpptagfqr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmpqvhcy.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkfobsog.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gcztovqon.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gxqgyomam.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhxyuzoj.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdauebcyo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghadryytq.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gtfxmgfan.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcinmcdzv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqstetqta.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwpjfhin.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gkirxetbu.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcybmnejl.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkydermzx.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gewyoxavo.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdmsevvl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/geuqiyveq.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/ggryusyzp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gebovwfxw.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzsjgqdt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gflpjbgue.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/ggzlczyhc.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtimgdnoz.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqgdamlt.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gkvflntxs.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsovkakyb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gttvgbpul.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gxxlsboee.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjxshneg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevlysgpf.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gnvmtgyje.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gcjccexsx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoghfhdj.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gzflbuukn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzavnmgt.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqesrhsv.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gefitefmb.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gervyatpx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gulkwqfxp.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gynvgronm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gizbyfjva.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/govrncdug.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/guihbbjzy.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gdildzfuv.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/goxauteua.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaskbpto.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzehvpeh.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gztuupuym.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdukfmmni.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gphvglluf.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoyjxnmc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gixqxwaxx.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/guzruhkkf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvychkile.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gfkwdaatk.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmfvmons.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcamcsmms.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gfpwupwtp.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gqtdsysay.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gdhbirfme.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gtxqhhxql.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdvuzced.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gndkitaca.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ghjdttnqn.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddnsatdj.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/geemjwsrd.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqcuncie.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gmbargfff.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gdzxafxte.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gvlmjbwby.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gofkbjmut.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gabejpita.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gixzfkhil.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gsnfvpyfq.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzujqzjpy.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grvivrjut.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrcawzua.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gbwfcyrit.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjfingia.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gktsoccyg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gwpxrjjrb.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gypofaeft.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gibztzack.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhobiabn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcghnoqru.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/grwrkruck.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaefzmxx.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkzcjqlc.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcyvunqg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfevmllhy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gezzjylyc.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/grgrtbucw.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gwapdkzzy.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvqgmkfx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gepxftdeb.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/ggpskxtzz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfoujwit.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gwrpetboc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbixcsvn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsogjnytx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gehgenxji.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqxpqvjd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/glnujqslw.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/glajlhzge.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gnibnuwgw.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzgburgw.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfnbrima.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlsicqgn.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwwrercj.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhqawdjm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlbrqkoc.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gohgbvvcp.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gmeosqyak.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyhsdgfg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gxahmaryo.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gxlteywva.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gygaslchr.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gelgtpxzz.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxddxsmh.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmlbiwib.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/geareaosn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grzibfusj.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxytletl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyyjugjr.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlujhtpa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/goyoyrgpy.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpngpzxcd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtzxrrpv.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gggksuoes.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjrekjmwz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqvginpd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gipdllcxi.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/goslznbdp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gwyqxqhlg.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfyndafb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/grmsraiyj.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gnaqnmpyg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvebfobb.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gzifrdvhr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbjsstww.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gapupuiat.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfabrguaq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyeixmkz.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqpkovtb.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkxkxcxg.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gcxzmewwa.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gixqfteug.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwyejies.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/guobngcvy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtyoucii.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzxegnfv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyrofhzn.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gctrdgoes.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmvadgnvs.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvicnvdvg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxklktnnt.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gtgeqpevj.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gukolhpbc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gtqolbnjg.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gjtvydjoa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gptwlpfkx.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/getgsjruy.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gceycaksq.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqcqpdqa.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtthbdnki.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazxbuurb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gztpttqrb.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gagjogran.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjonupqb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gsailcpme.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxnhtvsa.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gpdxaibcy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvgkfwwys.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpzqlcly.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzbnkjjf.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/guaoplkat.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbnznvdz.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzayzbqrm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gtgqjjaue.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gkufzmxfk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/grhawihiv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmkakzfv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzpbfbhb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gavspwvaq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiojietk.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbzaimfr.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnffuofle.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gbhaeuoms.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gppjbujqa.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/goiaaymrd.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/glaujoytz.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gyvpyxntw.sHtML


<!-- 参考信息 -->