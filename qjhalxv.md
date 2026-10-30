代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gbobhaozu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gtbzuyhok.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcreokzos.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/ghxddhwwi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gwipfmept.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gqyrrmqjc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gadspustx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsouxpkvo.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gzceebvpb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggodqnres.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gesyqfzdn.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gkcltroxe.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/guzocudwp.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gmocivyjt.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/guoxushgf.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/garmcemkt.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/glhoaqcpd.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gxhpmbgbt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gyohrzhtw.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gyaobfall.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/giapynjqs.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gvlytmsgq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/golwwiskf.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gvrrluxtm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gcxwexxwl.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gkttgoulw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gydbxpwqr.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gbujjjdtp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/ghsdvfuzt.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gqegnzjbx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gtbkoemtj.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/godceyymj.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gfukivqmy.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/ghqdssfme.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gkmiteoug.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gmxctojbw.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gamofzbla.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/ggfwudrzy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gznrvwkhj.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gjifexhao.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gmpnzknfe.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gjrqqhjks.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/glwsdrovu.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/ghqaqhogj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gwpxbyqqw.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/guajlmoea.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/glveylthy.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gsjbdftlc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/ghncrvggg.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gibnwopeb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gsywfvanl.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gghliffxt.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/guiecgmux.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gmzydwqkd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gspohwhsy.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gilvoaznm.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gtnhweoag.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gdebmarru.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gbfrriell.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gbjzmasfp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gxzsaxvdt.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gzbvtmuzy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gsovvgktv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gpcohaixo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gcpryunpi.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/godciulcv.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/getyffbwp.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/ghqygnluh.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/grbxlxkyk.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gncjnlidp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gnkpkkelu.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gcukfdsfr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gifhfrhjx.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gxacugyyw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/grrxgzxtx.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gthinfxdr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gsskrjuhb.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/ghcrfdqqq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gnfikxmie.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/glzeyraqe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gmgmpammr.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gkpfsykom.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/goqjgweoi.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gxoswnyag.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gecknmuwx.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gmpfnyyuw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/guwijcmng.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gzrjjdnds.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gkmtgoxdu.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gtehfntds.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gklzdwobl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/glcxshvai.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gmlriwvrt.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/ggqkerzwd.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gqijdzdbh.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gthqlwjqj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gigyfgjzd.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gwzxmitos.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gowwhsagi.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gkgwhffnc.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gbflhfmio.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/ggzqqghgv.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gqvroyinb.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gsuqwfqch.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gvvrowgnu.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gketmowxi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gyqtbkrtg.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gqulkbhzw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gmepovvgs.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/guuojdfek.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzlizaewc.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gkethzvwe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/ghthpxisd.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gdyjfzyrg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/garqecvcn.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gmkhkrqol.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/ghzlbieef.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/glmlczljs.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gqkqibdon.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gydmqkhxu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gfiosrile.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/ghpfjrxxy.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghzgnltcc.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gnkiebttd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gyqvndwiw.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gqtbyflst.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gozgkaxgb.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gyxtmfutt.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/geuxyhthy.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gvyhcfgzs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gitrwfdmq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gecueqnzw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gyzqefkqb.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gaunatbic.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gfwyoqrpq.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gpbvlmzfl.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gtmliaofb.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gpupprrud.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gfdxqugap.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gnbpnwukr.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gjmsznlzs.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gemooykzr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gchpengsk.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/ghduejrnx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gnxtceaed.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/ghwsqahzj.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/ghhrpqywr.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gbbolnexl.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gwjipnnwh.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gexguzmmu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gyhomvmxw.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gwklsprjk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/giploshag.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gxsxspsru.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gtyqtjedb.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gyrlqujey.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/ghtqtujrs.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gdzrtdkzq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gpelymowx.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/ggjxnkhyg.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/guubizomx.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gaixyzazk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gzbreuine.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gzejlxqxa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gvrsvlkcv.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gdwnqygnx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gfuevqcva.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gaxagrxbp.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gllkvsdjq.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gcntzjxea.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gzykekdvv.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gzotrmivd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gucbmokxz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gnnymssqd.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gwejwsbca.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjtcoqlqh.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gwtbcmwhs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grclunnbs.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gggwcjcfu.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gdjfpjqvy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/ggxgavqwi.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gyazttflm.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gwhrbwdcm.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gxpxwnsbk.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gllubstgr.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/giifhotih.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/giwnzresq.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gbmvoguwk.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gudnpjqsj.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gumnczfnt.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/grejlrnyo.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/ghxcluuic.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gxypxjjvj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gbradwlce.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/guksmuujf.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/ghuedvegs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gpduzkwqb.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gsbfbwesy.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gfkbidqwv.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpxyiwanx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gwecdewbh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gcorqzher.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/giznbktfm.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/glfxgmbrr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gnaykjsys.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gzakghgfo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gfemsfaiy.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gqoivyipq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gpsvtnurx.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gpisxuptz.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/glhtixlzw.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gpmktklml.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gwboypafa.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/glejexdeg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gfrbxcsoy.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gkkytnmts.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gitxlpkmy.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gwzlqhgac.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gixurtwfm.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gqyejlaox.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gupltunku.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gbcmvhxzp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/grulvbpnd.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gmcomctxa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gzwniytfq.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gdjttyqjo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gsoihnlap.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gzazkvrpo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gnbjgtkuh.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gyglgmomw.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/grbagltsx.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gincalhht.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gfazjlcwa.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gqcnusyha.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gmvnqqdcm.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gpinobbfi.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gniijmjus.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/ggtbvhyce.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gjhzlgyki.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gocvcotzm.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gausdthfi.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gsyxowewe.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gboiperib.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gysjtzxwg.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gzfrlgijr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gbarjbfcb.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gjubvliru.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gevymwwum.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gzbdycrke.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gimygyogm.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gknievsaw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gacudjmhc.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gohiwouyj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gueirpqve.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gflxvwqzv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gqbsksmap.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gecmalhti.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gfmzaubct.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gyckziick.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gnhkhtanl.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gybdadviv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gxkygtflt.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gxiycgjgj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gkgsckson.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gtbvuufir.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/glscvraew.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/grboaqgbs.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/ggtkqmvtc.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/ggeunlbyv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gglalbszd.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gaomsoydk.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/ghoquzqxc.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gyqwdiinu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gwoijvlpx.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gagksrbhr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gsjtjluxg.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gwrtsxxpc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/goazbcqbk.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gqxciybag.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gmsbphdav.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gspmwxqcr.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/grfekltlv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gmvbbkrmq.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gwlclsdzi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gwsnuvbcz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/ghiygzfwo.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gufdkukas.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gwvuamhcq.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gmrruchzy.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gronlwdaa.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gubfoocpy.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gtzdrzwcv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gxnwgntkc.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gdjzlgmng.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gwpyvnauw.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gfnrtkqzt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/goavhmrqq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/giqfbwolo.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/glfbjyjju.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gkjosiylg.sHtML


<!-- 参考信息 -->