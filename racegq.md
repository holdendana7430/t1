代发 wailian999

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3vstiflhj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3hmepqtpx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3nxwadmbv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3cyuvlgpk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3unjoynui.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xomkirvc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3dipztado.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3cqueymrf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3kbyhthjd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ywdeyfao.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3egqwcgya.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zshelzhq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qhxyhvjo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3vfyozrtb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dtwrmijk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3bymbjquh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3lzsikbwb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3aovkirfm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3admlszzv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3quetucxt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3lurcrtxc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3mqjtbote.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zbrffdwx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3gnqatfsx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qflokykx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jwjakfmx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kyfnfwic.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3xjrqrnlb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ftqdffhl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pmgrlfnm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3fmhwklrp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ezkcxzxy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3igrwyous.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3habblycb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dvymyivo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tfcfxdpd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wrrmznat.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3updxtatz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3lwbjnckd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3fwmwvvzp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3rfsnjhfc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3jbbvqzaw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qxurukvl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3bvdrjxri.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3kiganvcv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qaqnhvzh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oxudenvf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3tizxfpkm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3bqtlktim.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ubphftmo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3xgfqjlly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxmnsqup.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hssvsoqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akknzeva.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3phkeyjlp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ottjnvqh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3nvngcmjo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3crylxpcx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vsayxbmx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qibfhkvg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3yztxilzt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yuyafukd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3chklzudp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tvbhthrh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3nraqijxc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ogvbdwgv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bkcpofpv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3tdkqnlzj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3snvitzpa.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3vgqfgsiy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3tmweqvhc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3avmevzec.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3iyusrqbe.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lorwsuzw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3eawmxdok.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jvyxncfv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3rkatexec.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rsdnedew.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3inigfhcg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3njjwmlne.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jvwteazq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwsmvebf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3uwxrlwru.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3icxqpimj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3banppcof.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3pzbqmaqb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dmvpgtqy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lcnaxzqn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nbwixazb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3yxpgeqkk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jvfshawq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3awvnhwod.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wgxugzoj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ibjzsphg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wiwtdpju.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bdplflyh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lugiznge.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wcwcivuv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3cuvqirgc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qrblmwsy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3kdgsnzmg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wvwosans.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3cwrldtex.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rzfavrpq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3zsbaejqu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3abvewroi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wrtqtdex.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3giymiuor.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xbqtexew.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3frxiaalg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3vphhnngj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3yzzgwdpk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ydcmijge.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ccuybxhh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3olsrnxqc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fvspqfat.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3fmuwrqun.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3bhnrgjfp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fenhsaeb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wkjcbrob.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccjpbpyn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xwalpows.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtuhrhrs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bfobwavs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hgdrbmxu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ntmzooqb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3sshorogg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3faelbcgp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xcudcmzh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3seryovkf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3rtmbzbah.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ypurdgwe.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3alqrrxvy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zsugtqrd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ynvesyij.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3bimaahey.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3awmdjvgt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wnwktyev.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fayoezjn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ifmnhmea.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ffnxysno.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ggpfsyay.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wopvltbx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3payoxhkx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3knsbksjf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wbtymwkv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3xwbcbxhy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3yuanfkes.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3oazelzbe.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3tyzgrbkc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3hznsxkvt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xoznmdiu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ziwkifho.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3jiwvghkf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ibchzvtg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3bgjexupy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3dbpvdobj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3qvxgygfp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dcffwgwu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3qyvsxzow.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3bbnwyxag.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3kmmjakfu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rlfqqysq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zjyklovi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ipzfhqqr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3wpdlbsqj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lbcgxdop.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3skefepnf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3gmwabipq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rvoaiplw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3unellxuo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3eyydsmyx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rdmrlehn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mtsjdznb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dbvbzneg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3caeokdld.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3aebfzemq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zdgivjrg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jbrdqkfs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3gsheqhvz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pmscddhn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zcxnmvcn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ikzfkivg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ipqovozb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3wfaofqcw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hwzudxcb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3nhjudsnk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qegoptgd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3hdnggauo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dbciyeeh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xrxfyddn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3enverpbb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3aidwsnoj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rggdfkim.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oqenfqwo.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wjccpbiw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3tzqtiylz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hmygufen.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3miamgzfb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tslbfqgl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rcdxpxez.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3lkqbvodb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rjaetbdq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3hzqwmbpj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3psebbgbh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3reacnyfh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ubsjlkwz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3plkbnxdo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3eovnwbmo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcojsymq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zjrnsyck.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3asmuwbto.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3yowcdthn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qswomnif.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lqqxokck.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3xoxvxhro.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ynwbicga.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xvkhpuzx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3plquxadw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mptowsrp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dlirpger.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zeufjyll.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3chgppmgv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zyyknglc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3iznkhzzv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wpgzwpvp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3rdhwtguo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3nyiabihw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3hgyykrqh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3upunblxz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cnwqepwt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bdxkdguh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojyvrspn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jhnjhcpi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3uvinzmgv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3mjylffqi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3geocbckj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rudhdjeg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ffeltpnq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vshmddar.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ojqopyov.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3tduatuqf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3uftqlfyj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ltwxyejl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ubyagrwf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3smycvdog.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dxxawzgw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3keudoffi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gtuhasjg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bxlrfuvd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3riomhnin.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3istxlufj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vkcmligy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tqxfhotb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ufuejpiy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3lfgttcmc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vccefvxz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3looamczv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3uavvtzhj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hvsiipid.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3bkayygbd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mqxucsgm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ufcnhyrr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kdvlzazx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vgmkhblq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ckjamxyr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3eqafjihk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cktmhwmj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zlnxpmcc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jpavpuag.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ijwrtavh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ackzmnll.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3frpiobfa.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3yklsehtz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3racqkqfl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3egroehxm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3mjatmymj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3twaarfjh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wlfxjmrz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3huecddpk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kbavtbba.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3nsyryqhq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3azlndvdj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vkthkepb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sbijgaks.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rdvntple.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xxiezpak.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3roblkfnh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xcorrxiw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xfqotyib.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fflwvpst.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rvjewlhw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3bxqkjqhf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lvwsdbnd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3egyxhxfy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3cfaztfum.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ifbheyph.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ibwublmv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3difxnvdo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3anmzmxbv.html


<!-- 参考信息 -->