代发 wailian999

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2queftrfp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2fqynkxbl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cytsuxzn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2tmhdphfy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xdqfwmax.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zhnleezs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dnvzeeth.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vgxjkgyu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nzwxhmwp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xitkjxhg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xxmjxmaf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2lkpdihdh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ttdmntiy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2varbsnso.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2btxcoqgu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2uysumhcs.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2dthvllbq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ngtyuejv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zcsmurpi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2odfbanml.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2couhckki.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2udckdcbf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2atnmtlgd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mtuqjvla.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dqabneho.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ovmvtaag.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bqghwncq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zvdksgca.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wipfktbt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2plnvlhqw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gzdwatcn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2apajxshi.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2nhqulooj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2iaymaykz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2jptuweyq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2cstvjyal.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2nemxclvb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fcultaqy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mjcbnofj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2eprhwtkl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2stgtmqvn.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2lteceznb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2sldrmfee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsknqrbh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qgyobtyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdpqisxb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ezudwirc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lizalgca.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2woiebkrk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2zvixpwow.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2unkxldzu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nmencfrs.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2nszztuex.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hlcpagkh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2oiwvquis.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zrpmkvbp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2mfybjkks.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hukiplrg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kbhtjhck.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2whqqueru.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2uunubvcc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sdkjebes.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2fukxxrpx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zjkvqqwf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bddzvrgm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qsissgwa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gvehjbub.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2pvuqmykn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dinwhsmn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xmugubvs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2abukaurl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2oxhlwlbg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2zippzdxc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2fclmzmtd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jhcsbtoc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fozhvzst.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xeyhdyxa.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hjjgltih.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2moxearrt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ztfwrcyg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2umglrjvg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2nyvjvixj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zdgxkrcw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2igihxyvv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qupwbbtz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xjqwkjyw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zazpnbji.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uqojbric.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xmkusvjj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tturoeoy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2iqypeymu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2axlpupum.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ffpkvozn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2oksadezu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2elxcjbso.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ukryixdz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2xkrxjzhh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uqrpjoyq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ygyaemfl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mcbrqyxv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2sbfwucpb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2yjbjfwrp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2mpfnbzyx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2pqcnlbys.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2vsqaolew.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ftwbqvuk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ditoyhgi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bkfgljjr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2wvchblgw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2neijbeci.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2tbuhfbrv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qffpixrb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxjwmkji.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ztxdfvbb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uwaqgjds.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2uovcmfzz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2fgtpafee.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2gadjdzuw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2avyxnelt.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2csgxfqrc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2arfxagwc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ahvbwsuc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bemkaqvv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2rkhxjhlu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pncswtxu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xzgnuluk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2uprxqxwa.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zpmbevql.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dldvzapb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2tifplcii.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vajptjmu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2piccgbcv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gbxjrsam.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2setyxxbj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uzkhpykn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hkafbbia.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wjmgjinp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2tqhbcpkd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wgyjpddz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2fpidaake.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2kzqmrquy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ylcgsrci.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zhrmsrtv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vjjkvbvt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yzchdftw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dcclhblm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gqdbmjve.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2zvaomjfz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2lkxbqces.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vadowvtu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2widraupa.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2iyuppehy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2etujbutf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2btatuzgg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2yosputyl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ielpjwri.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2bervpwbn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ktippiut.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2yqtnbsip.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vmpogbwr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2maqzecof.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kcgevjjz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2baieajhy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2nsunlhet.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2oesttgvi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ajahhxvb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2lhxfipsu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xinfdezl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ngzedhhs.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2veyarvvh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vysjlvbd.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2wfiaaxof.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2udlshryv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2cyzsoojr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rziapzpu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2njomzohh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vtvcjhit.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2hernompu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2yzydwuxs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2abxmnswv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2wkqiiaob.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zplkmnls.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kjvkokkg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2pgnrbcpp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2twhliunp.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2oluyfsav.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zxmokmjs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hmojwmoy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2rwdrcvfs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2whfozwtk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ofzcdqth.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2htgdgfan.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nrzrozth.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2cyromsjo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yakncubn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dqnyvrmy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rcvdnfxr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2yigbwcmt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kauggllv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2psxljrdn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ijbckatj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2itynghwe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2garkwyna.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2wtpgbqgo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2jjjdkpat.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xatcxdav.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rzvgnzri.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ottuxhgp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vcpgkomq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ebzqvudz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2bghpndrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2savgdflm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bzyswgqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hclloziz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aerdzclt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2zjziicbs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyuvnumk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wyxlfcnx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vajohlqq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gtpokvgt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xnboatdi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qglweylz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rvghvxlc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ffklvoao.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jggymspi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mqyxlnlr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2sbwoajbj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2svcemqzc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wravwlav.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2pxhdvvcy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hkcthhjz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xpvszfjg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2unswlcdm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2olndbzzy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2moqtlhiy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cbbzokub.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xkfwavht.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vicasnyw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kplrbfuu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gdnrxcbn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yuexmpku.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2sksgomgy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bqlkabxb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aamgszfx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2yaarvbdw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2mqfwhbag.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qjzghigh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xbqeiuaj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jxbxqerf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kpkcrdlf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2pmmuqodl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xrbgvnju.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2sunuewhf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nmctyjdl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bbzoznvj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2lwkrrekm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kbxeimxw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2iwddjtrz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gvufgvxk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rklkobor.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2faloowtb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ebmwmgxn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2fyrvlegt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2cwbubdio.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2kxlabyxy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ppvidxld.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hhspwkvz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ikknuctb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2eyqdipyd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wovcdags.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lnynbqpm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lnudihgb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vttnolar.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2nntrtzjk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2aiputofu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2dlbemkjp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mwratfvw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hdicdpwm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2trurrdam.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gaxcvzon.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2vogpeven.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chajhuks.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2desnoiot.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2sgwnyiwn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2jasosdtu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ssnxlcpr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ffkfffyk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2splpzreb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2nhkjnsbk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nemhfzwg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ietrbges.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2swqqcxcp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2kouzwnnz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fdjxfoer.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gbflnbrl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nqijtvic.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2fmgqlvih.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rqfdpgbw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qixolvlz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ckjnukin.html


<!-- 参考信息 -->