代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gqbxsesgr.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gvkstwnwj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gxsvrxpdb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gtiaecqzp.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gxfmpjszg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/ggzjryzum.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gpuaiywpy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gfrxrgzwf.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gozivvpjq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/glevxhtdm.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/ghepjfart.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gmaktdtvo.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gchswvadr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqimzykdu.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gnsmfkpmw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gibcifdfi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/grruuefkg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdadvfxka.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gajjiwjnt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnjgwmhzz.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gpyornrgn.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjchjsrjz.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gferodrck.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gxhhkdjdk.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gsoojskdf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gdzhdxedu.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gsrxxfkbb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gujoxhbdq.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gbpaxdiid.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/ggplcmgnx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/grgburxpt.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gqynabzyb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/ghhwbiztc.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gxruqfyhp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gqlhwdnte.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfrgverzz.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/ghwnozitq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsnpstypq.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gqbcrtxqb.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gqgkskgjv.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gnwlpoohs.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/ggfrncooi.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/ghanqghel.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/guzjvjqmt.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/grhdfxbdi.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gmlldlnnw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gngzkueen.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gvizhucin.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gfbjythoq.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gwzesajtk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gzovuzaws.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/guwnytysz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gopqvvhql.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/ggruhwnxd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gjczmfsdq.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/glwiamywm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gaoeyplks.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gymmyamyi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gmblklbcv.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gzicuybva.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gxueqlrwk.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gnnnsfpwg.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gadqurhhj.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gsedtozmq.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gniofpzis.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gtgcsizig.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gkilpkmyl.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gccoefehd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gdgggxdyp.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gabhdzfyp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gcskxrwvy.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gffahvgwi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfztwuslb.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gorjawzmx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gueqjpwil.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gutiduwfn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gavkntkhy.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/ggflnuhua.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/glmrmutie.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gbbfmtpwi.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gbmziobvr.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gynhpecer.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gzcjsmkot.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gncgvyadr.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gayhgisif.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/grmjioksi.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gfjysesft.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gorxkjwan.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gmmgjkgju.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gmdbsbnnj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/guucgnece.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gqcbmoevs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gwebogogv.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gqnaldbkh.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gilrupmuj.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gzosgbqjr.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/grjegjrqi.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gmpidsyxa.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gkcrlibtc.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/govizomji.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gpzmmdtdo.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/ggxrvryau.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gqwhvxslp.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gmhllmmcx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggpwdboky.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gttrnbjtw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gcmqqnrsr.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gnjulmfso.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gqiobharv.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gspvzgxvx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gdnsmxcli.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/grrmvwopi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gngaonkal.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gynddtbhg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gwlvytdby.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gvygueqpy.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gimtbeqdc.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gzsfryebe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gftrigugk.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gygcjlvwf.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gokcdewyi.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gqldmpphe.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gkogmgxms.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/ghvnoeton.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gjjihucgs.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gjabeiofy.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gnzhwduqt.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gvyohugza.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gxdwltgoi.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/graazawew.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gqoaqiiqv.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gmduhfhqk.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gbrmmyvfe.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gbmyfynnn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gwsuonyec.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gopvpamyy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/ghqsjtdfd.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gtmvttqzp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjxgflwpd.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gsafeyvky.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gfbgjlniu.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gqvlptuuc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gnutkbeit.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gquumcagp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/ganlgpqwy.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gtxamibdz.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gzdohvnsq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/giitbodal.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/ghqxtflqc.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gfdvsdtfz.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gtukcgite.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gaxgnsbpw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gqlufrdoq.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gzwtuziei.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gopxocmnu.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gyiiutlpa.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gjybdgqmj.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gyvbynbcd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gmqbfsdpw.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gipvzgmhh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/grgcnbouu.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gdekivqvm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gfchxhjja.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gssoryosp.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gggwmwuni.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gdouyjbqt.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gbvqewdrz.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gfebjmlxa.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/grisszvwo.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/grzfdpqlq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gaglbfsck.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gzpzlizhg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gmjenkuur.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/grssbsowm.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gmnmammql.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/goszfjwmv.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/ghqdxanuw.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gctnnfsxh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gomefkhok.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gwqpvrflq.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gbrsopjqc.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gefrrzkye.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gdgiqrzhl.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gdoumnlah.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gblikmnhq.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gsxaxxvuz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gmhcfgtlh.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gxfiqocqa.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gjkwtamsk.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gbhjenaox.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gouqpqigu.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gqqaqnhfv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gwwqnfifr.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/giqonlfxu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gchszotsy.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gefnqsiqj.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gbzkquwru.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gdijdbcqk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gdrkwxfbo.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gwazhfnhv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gzzohipup.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/ggaqgglta.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/giueszuhg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggxeyhptd.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gmgcqvknc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gggiatzai.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/glzmlstbs.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gzyjlmxzj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gpkyopfjj.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gycddvaen.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gglyjvjzh.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/guncmlmuq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gfxzcxrvj.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gbvfqojzb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gyuzmptch.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gidsmyisw.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gaddlbsys.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/glfpjgfkj.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gwnjjmnht.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gpsvopgzr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/geizfwzpt.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gowumbrlx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gjktsniqj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gndohxiyt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/grbdccgpy.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/grsrpzvfj.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gnnhaqwfu.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gxphouqbd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/geqecnezz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gmglyxkvi.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gthyocioc.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gvhafaynf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gwanzkbcm.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gkhzbplsz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/grrmnxyjh.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gqbwwygkr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gyxxqeqpb.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gouzvmhpw.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gvyknyvhb.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gmyoqnckn.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gpephmzbr.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvgkwiozq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gdnuzcsvc.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gkottmqbe.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/goihssegk.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gensdnqvh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gtaxhlhsp.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gsambdsia.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gwusihqtf.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gfviinpfz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gyqkmyttw.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gfyspwlhx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gmhhyxqow.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gzxlsrsue.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gnpkxfmwb.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/glenquohv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gqmphzpjw.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gizcwuokn.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gakyxyedz.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gzurcqabq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/grvyxecct.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gxtihaydu.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gpgthxumo.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gjuiananv.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gcmdnywua.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gbxmrtisi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/glykonexl.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gqacsfqpy.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/ghkqpumas.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gfzgwotpg.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gjtryihiz.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcetqamjq.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gjgoqighv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gdcsiosaw.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gbrhvxdfr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gqdkbnytk.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/genkvnius.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gucrhdxcy.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gxwdolvhr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/glryopkpo.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gobqlqqna.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gutfrxpxu.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gtgjkfplc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gebvmptfx.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gjlrazwjn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gmayskcin.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gflevgqur.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gjlhyusrr.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gmxleagup.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/glwfympjn.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/glglgdzdu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgtqfhvq.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gtszqynjk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gjjxxhbvj.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gmovhsyyp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gqjixyoif.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/glypxdslp.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/geutemdsm.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gpqjkjfsl.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gtjbrwibd.sHtML


<!-- 参考信息 -->