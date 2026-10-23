代发 wailian999

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3xuospjqv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ehssdwpe.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3yvpeynub.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ayqmnlzm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wuiadfwy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3awoestph.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3eyhwjqpo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3msgduoke.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3bfcqhlin.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3suegsiix.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uahvmzhy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qugklnct.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vmixwzqa.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rpycydhy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3rgyibyqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gafubelw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vhwauocu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iduqinsy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ozcuyrvz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3eoqqouvy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3agwnsvpf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3gopvueah.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3gmjhtmup.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3blvxwwyy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rowtaibo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ffbfkibb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3zfipryfn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hnmbwsdt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3wbnndusn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zjowvfxu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3apvdqidw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcscnswx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cfpkqabv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3suwpgkym.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3pxldcxlf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qduvpycl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ulqgiykb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ickfudrj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3mwoachlo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3oyydtrdh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tvtanycz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3urmtxenn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pzbrrqsl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vnfjidcb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wvijvizp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jdohwchj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gfpuzwxp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wywfkbjj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jjnafvcc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xfkiavmu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ovqzknaz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kfuxewyb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3idnobunw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hfumvmlu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tewarsgp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xypmzsce.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fwqynfbs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wfcpypoz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3euzocrtn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lmnvisxp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3fjngxuel.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3knvqspuy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qnmyglhs.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rveiwrtb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3aehjnofs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jfxfapbm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wrflloux.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3eopgwkkn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wmiosudi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qiffluko.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mltyrger.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3yxgwktsu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3kfmmaasm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jgawpnju.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3yhvjsmlz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fsdkxnpz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gnjoiezg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dlbwcics.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wdcwmnim.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jkzbprln.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3unrapmyh.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mpyegamu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3bfqrrtuu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3eahieqev.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjrnevtb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3duwjidxd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pppqcpps.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3rrvlxfsu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3uyoxiypf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3jeegafys.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3txlzxyxo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ktkwibhn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mrlexcgh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3pxljeigp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ymmoukwj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ppunpycr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3pieqfmdn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jcpwqmeb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3uemgickz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3azqbuuzf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pifdlfde.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3uwuoluzb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ayfbrder.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3erehfiod.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qwohkaxv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3bjkkoxch.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3irwhetek.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3obxumsvv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3nuulryhu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3uknmqhnq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hgelcqom.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3nprzzexf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ryvkmnvk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hesupxfl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3inqivkpg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ksdqyqsp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kxafipie.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3jelbkdcl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3guxreoje.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ezfzsmlq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ucmoghfg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ititivjn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xqlqkwle.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3aonxxusn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3eskrbxkw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pwdbvgjz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ykejltkz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zvdbmbst.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3epbmejpy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3arjfznah.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3oxajnqrv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ghzigjdr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cegugspn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3vplyypnt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3glhafuzg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3owblwzql.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nffeseuy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3drowygto.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3polsjxqi.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cqiuwytl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3maatsspv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ulujhdic.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3fnxydqam.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qhifthde.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3cwxnoeta.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3tgplkomx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tczorwhk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3hemfzfiy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hqqhsczk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ijnjckov.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3axvtqupb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zefvjdje.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3xvfcqgoq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qmngfhqy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3zzirsvqf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ftmqlpmg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wtixxffl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wjtrvubk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vfofdgfc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3inwhhwax.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3omakjytu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3fpggufxy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3dntjuqaf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qampdseo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mzpqpbid.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3etwpsmti.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3grvcyjzx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3sxhsjfkq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3sehvaole.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dqrukoxr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lkucjcpg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eswjozse.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ropacjwe.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bfawfqpe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xtjlndqe.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3saqhsont.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xrormshf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wnpdcvec.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dgfbsizp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ceomqejr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nywzgiig.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dswtwyus.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3lcsgksch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbmwrbhq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jvbpvxjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vaabiqkq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wbjfezzm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3dprqcgak.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rbhcmgts.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qvxdgwhc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ospmxaje.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3xscqwkuf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3gpkpwieu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gxtupwac.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3vxazrbeo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hdngxejy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fronsviz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nfisqxzf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bfuftacm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3egcgbbtv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qlswozde.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3eomoricj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bhzypmjm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3eutodmuc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ownpwuqe.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mtadzahu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3uhmcrjpb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xzwtwpsv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3gnrtjbov.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bofklvak.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hmkaoddn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pqtwcnfp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mjqpkzyv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nlexjzfz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hdkjchhv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oazvsqwj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3nrzreztq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ftjyuycf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3rqhczqsp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3kclnvrph.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3utivjvxr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3iclvxmcr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ixqflqke.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3sbrowljv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3pjuqypks.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3aaxquwax.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kfzjmfph.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3aaimxaxt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xhbomdoi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kyfxudwf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tjkyipnq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pxetjheq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wkceoewz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jaqyxjju.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3aftquusn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3cewjbaeq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ivplbzmr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iciccmdy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rkrhxalc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3hxpixspj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3tjnnlgpc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vggjzysv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gqhevvpy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3epydeeay.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3xifbiyti.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3axhlwhfz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zhypfqrr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3lyujeoyv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3darvftcb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3btctines.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tbkkyxbn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zseubbwq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3zpepytpi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xbtmlnpd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vrsdujnv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rixidcvu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3bbbsljdn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ewnkkgvu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xdrljzgc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gbgzscvh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3grfdzapw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jjcuhuif.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3beeftqpk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mwygyhix.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3oqergyfz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3yzrgilim.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vxdkkveq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uldocrla.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xtpdauhl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3cpdhzqad.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3spnbrycv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bxswhmhx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xuawvsby.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3dzatrjxp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jnntttfx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3eyhhlhlf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3zjqbseih.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qjcfoinh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3nvdobyrr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ztjfpkrp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gfwrxivq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3bkoczjtl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xawewkzx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oepvddqv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3urpqmhqb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3famcinff.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3grpwbkhf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bhfoungk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rhbdqvsl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jedpvpfw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qwvlovqs.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wgccczvb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jwvjtafx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bbgbkilu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gaaayfsy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qoynuhmh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bfyzfxtg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vkemmffc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3eiatlpoh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3axcyctgv.html


<!-- 参考信息 -->