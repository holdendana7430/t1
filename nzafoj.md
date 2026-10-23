代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3atbgaaft.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3mzbkmwlh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3nbsrfszo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3aylmjiiu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vigihmax.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xcqwysbf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xxhakwih.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3taewpont.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3znrqvtas.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3twvmvamq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ijrupvnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bphwjzni.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bxkactwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsatjeya.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3cugdwwmo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tfpxrilx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3nnltfook.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3kxkosfdp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zskctysf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3uxhuanaq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3zgctyszp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3rjkimvia.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3zbgbctdl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3brnvnnbr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3oibmmajj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hmkmwtyu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bazkueyn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rxfvxcah.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3bmtqhyxy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rzeaayle.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ulsacznx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xqdvkrbm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rjmjqmrn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uplhpvgz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tiyhlwta.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ngyhkzhb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3uuaagcke.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nucapsak.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fqadjwye.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3cvhfgmiv.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zhwglxiz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hrvxpbrt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gecxaaxz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kfsmxlxs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3oeyuuhrl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3fudefjej.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qtbfvcex.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uzqpakjl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mzkucrze.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3niyrmzmj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tfubzprg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ntfdhfks.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3mxunuvlh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wphnzdhh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3kystryvo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fibhvmoi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3nnkmygyp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3oivdvylm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3iochrayx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tbbijmyu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3lwxextcy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gwttzpbt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3fcxhicdj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zxyloiec.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3cgsjteqg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3eolvmaay.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mwaoisgx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3sloddeoq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3qwvxokgz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3znotqbra.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3iowgkssv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3webpvbqz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3lhjpomco.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3elijhrjb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zpzbartp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jloubrok.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3afgcdmdt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zgjzwqie.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lnhtfrdq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mpcqoejr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3iflhiixa.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3msjkiufw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkdtdsxb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xumhkeya.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3tqsryxpy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wsfndszz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3erysrxqj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3dtuuatip.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3tljivleb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ooyywecy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3iprmlsmh.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3qllmbrre.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fnbbqawt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3vckvmlef.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dszenkoa.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3bkuklije.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xjvttitc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3cgkmbidk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3uutzcwfa.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3htsyxcno.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bgatrczf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hkixbwrd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3smiklfnl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mdwcgcge.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lbzipcmx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3uexfxyej.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tgzqeouv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3hosduwmm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3aahzvxbq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jwqrszbf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3jzolqjps.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ppggviab.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3penivflv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gkjzgklv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xwhvdonz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3vjdkdtcj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3yzqyclfu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3cxkitwer.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3skbxquao.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3bpezffkl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3nleoltss.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vjkosmet.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zzaurdda.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3bwzcrbry.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3gxoovojm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3qpsunabe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bqdnqjuq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3srtpgqsg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3mqhwefht.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fknmhyyq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3yblifaia.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dazvtlcc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ykvmcrkl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgdvzprj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3nvipofix.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3iqbyvmss.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zpmwtuhj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ipwftneg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xpfiswuy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3pmbpeulr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3codwldtp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ysobjyct.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3wvorgdzq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3amaqlkpn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3zreplgws.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3lynbqimx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3icsyigms.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zfzjyncs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3jzbwvjud.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ntucugfv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3gosjhxif.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3lrflvgfl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tftmrdpw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tyvhcrzd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jawkizid.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3aejkjqqw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3javgegpa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hcnbfgcm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3luhfyxqd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3icpmgkxp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ivxzgxxk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3clvkaiot.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3klszamuh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3tnteveri.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ilodvizy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3woxcbxqu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3phkemsgf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tyarjzxt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3rrtzfznq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lnryvysa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3aejxtmba.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3sllgkwtq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xgxmzkkf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zczzptvi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3crqfbvhe.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jkoztjga.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qmgirzuv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kzlfhkxb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3usacdetc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbogqpcy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hpnoppaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uuogoydp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gmkmwece.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3svvlufuo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tumijmbp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ernwxzqc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3zeadffur.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3rjmodvwo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fxrroipi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3icnxmomv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rfjovmkp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xdbpoaqv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tqihkzya.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cfuuzaad.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rlcgyoab.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3roowpcwn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zsefuggy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3uflgjkjs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qzppoiap.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ekvubwzx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3jlwoqlhy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3chzkxwhy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3gyzxdzwr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3roxowule.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yrgkixmq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3prlfwsbo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zladzuss.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbkzzzhk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ihlscwxk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ywkqglmr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3pusaoxpt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nhnulqce.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ybtynuqj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hgwspjaa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3fjmywdtb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qrznumlw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3opldswba.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ywlsazxr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3uqwtjuuq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3onbpibak.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3shtjweka.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ecidwacu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zgvudmpw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lpnqeemz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3khehkksj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3unvbhvuc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3gpsllcfq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lakffdtb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kwaezrix.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hoxywatw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uxfdtyjp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qmyuamid.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3tglpbubt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3bkpdrtwp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ildmizbv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3begcjmbg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3bmqdkezf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3cgunpxgu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yiaqeghq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3lgacfrbj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3eksbpgon.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3humhtsgi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rixnblzv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3cjepxivs.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ofisbiac.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lxylliol.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3smybucnq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tnvzbbxf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3niqvymtp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xqihkkld.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fsgbwoed.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3klzkwxwh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3rkxnaoma.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3eoabcllt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gnnlabdl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vubueiqb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3nzdbenlt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fxfzcovn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3svxgiubw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pevgbvny.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mzeyccpa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ljsxoibr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3omzfvmwu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mokenzkc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tmcwohtm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3phixpadm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3bgzvcxpp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yyelxddw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3afoqsumx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jjpmmquu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zzsbwwbj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3scvpwtoq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lgdbghxv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gcpcphpc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3jvkiojhv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfmnreho.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hdicsicb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3xkjvtqlp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3wntanvrf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3opggozmr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iwidnjvj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ignlxcvv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qcutocqv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3iosvqyii.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wenkerki.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xavyarsx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ciatmhqz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tfhwlail.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3neuavidg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rhbcsepp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3oihkdujj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3vjvbbblz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuvcjwfn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3hxbuwdyo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3vymjrprb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3bhrttvpg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yriudlbm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ttgocpjg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jztcawhp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3pppxvlsg.html


<!-- 参考信息 -->