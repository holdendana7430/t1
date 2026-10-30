代发 wailian999

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gtdhpnves.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/ggtszlxkx.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpyceihg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszzyohuq.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gswjtmquo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyzsbdkc.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gamvjpwba.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclekvokg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/getgetxpd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcajtfxod.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gvvdkezvr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnsgbambp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/giojmvxal.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwgelvfhs.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzephsxqz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gfljxizlb.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gkktfraxv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgjhblpp.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaogmoak.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdscodcnq.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxouksyh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/grfonafhb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gitnazvdw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gncpcspwv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gcugxtuvj.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gybizcnmy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyoqwlbd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gatpftcbq.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gvhcbfbcg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduypkgas.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gbeqriyxk.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlmyktit.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtndnxbod.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkvmlhpn.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gntbxkpde.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goknksisu.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gszvtbwdi.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunbzfpcc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkjbedvj.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjniftsak.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvdezijtk.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrjqqigz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyvgfrgn.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gevkzvyew.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrpegpss.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvptfjkn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrpnovxk.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ggirwuely.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gvpjegego.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/guxmnvawf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzgbmeiq.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaofzxrn.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gvujfoipk.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxxwmjqb.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gambliiyf.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfwayerk.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gyrmtvgzf.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjunaadeu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtnyqlvs.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gvvcyxvxp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtewycqmm.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gqamvumva.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsezimtgp.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gazyaszny.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxxkbgjma.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gkiajfoyr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gyabggyxf.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gjwuuajmy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbdpdelu.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcvwhjxx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/glpygmket.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gxsktwumb.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvwcmtvxo.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvnozwhd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gigvbjkyx.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggapcwuyc.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwallbwwh.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gakxwfbwi.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/getgdikbx.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/garmwxlnx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gknbzjfvz.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlelwyux.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gegibweji.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gsqvdkohd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkyvjzac.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmcqhayl.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsthenju.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gojhgrhtc.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/geegoelsa.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbfbgsrh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/glghfphbj.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glifyujga.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gckvevqnu.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gvqezaxzo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gxyvkyugk.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmizjqvpl.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyywhgmej.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gqgvhppjl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlgkkfbk.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gryvzkppc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gvomofbfg.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwbxqjgo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gcolakddq.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/guovrabfr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkvjyxgg.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfqngdks.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gkzbrdqqd.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdkkehyqa.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqshawiqf.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkhmxtrd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwqwdhxu.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gajxycqdv.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gzdxfdrhv.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/goasiozsp.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/glebpwmlx.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gftimzbov.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/goiydnsju.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gzxiixbli.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkkoyvdx.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdnihcjz.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvunahdxv.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkrqscax.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gaalcipny.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gabgkzpsv.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gdxrqykpw.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gqmfnzeul.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gkewdzqvg.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gksojdvgg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaoivtuf.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gflnkqmcl.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzfjtcnj.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gcpzkquez.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gnzgzipif.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gbieacucw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoqpwptj.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gicwatlre.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/grjxwqqcc.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gprzkxvdh.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gurzgjpmx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gaovzkvbh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gldcpvngz.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqpciqqs.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpyuhkfpv.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gnrticfmd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gqsricfzp.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gjueiksjo.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtorawcr.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpuqochu.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gujscgkjm.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/glpzmvgmk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gozmzenfq.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfaamxev.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntvuryuo.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/giyerzecu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gjypcyttc.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gbegyzgwa.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcojtzfwk.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gloibrmyt.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnaxowqa.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gfifjcbkt.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gtmypktmp.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gmvqudtsg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbixveak.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnynrthnq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnstouuye.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ghogzdchu.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gqdrdivpz.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptlndpkv.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuximcij.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gyymmgxxf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpeovcbnq.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gkyhhphez.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gpdujhuhs.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpawkeet.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpozqosa.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdizekox.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmmjwgvb.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsbikzef.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjownrbtc.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gxssqehmy.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gagpoffmy.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gsstbtmfo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwiyqvuby.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gaelxpeqf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzssimoas.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoihgdlp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxccrvxmr.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gvudnxkgi.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gcscnsbeu.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gnciplueg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkpxaqbwr.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/grnsvstna.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlhgqryj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrytcbib.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gumcnqvtq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjxuwndw.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groayddoc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/goqthlmdv.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gvxbqjzdg.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gssxumkmy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grbcmievm.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gjemgopbe.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gvynpijtb.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gwcsihigx.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuisyhfp.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/govxudwrm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvjghgej.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gqhfceaom.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/grvnwghvc.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gqqnuntpi.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gtisefxii.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gkktbeubh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxbpspol.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gwmlmbqqc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlkvuwrn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidcgomdr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gboluhsjn.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/ghlhvyyyl.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gvdwrsdqf.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbfcfoxq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/guucgbwcs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbldssuoq.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gumvjlzqz.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqxlltjj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnudhtkpc.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqhryjlf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/galcrxzqo.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gitbehgxk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxrxtjub.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrihzlrt.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuigqkkk.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gykevgwry.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gxopwvpju.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbknfydpr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gmsgahosw.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxysrvurf.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gjiostkgo.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gdntdyzry.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gzdxpqvba.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gajzjgrqh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmmzyarn.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gvxjpakvs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxfmhrgd.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gfksrfayn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxotioom.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkfqzdbs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gwhztfvxn.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqvjjixz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmddhqomm.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gfbrdqxum.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gvmaldtcp.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrjqazdj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfbzqckc.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gxmksfxcz.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gvdshujtg.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxjmvbtqh.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbajyeazz.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gihrmhwym.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/ggypouqaf.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuzvmgio.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gokinvigc.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gichxvjlo.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gwmabwqdl.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhxiuwey.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/groulwdrv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbkcceshs.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcgpxzrz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnbtgguo.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmuwvddu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjkfqdrt.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gxcrfwdqi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrdqvjpw.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmolfilp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtdmajlbt.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gplnshsop.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeoromls.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/ghphbijrr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsltkyiwy.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gbovfhtyz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gvllefgso.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxliipbqh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gmduxylqo.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/grabcplmq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/guhaivrbp.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqpothpsl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gnmpznqzl.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gccenufwx.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gvieufpos.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnwznjik.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/givyxtxou.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqtxxfvo.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givttozwi.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/ggzmeccdq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gvqowohid.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdljzrek.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoghkskb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwfrejwe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhiwddsi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghojcxyga.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoflfyox.sHtML


<!-- 参考信息 -->