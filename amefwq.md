代发 wailian999

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zcszssdf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3uxjktnuh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lvwwxafx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3cfrstgax.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fenhcoxb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3arpsmvpd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lfahwoyb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3cvbocimc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zuavlbfg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3jhndfcoj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3megsyzhl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jdxkoyxz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3sngajjye.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nksnwasi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3naloafmp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3rcjqcvyq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ivszmybz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3bmdsfdck.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3odwqqbql.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3avkbytox.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3fqxmzjoz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3mxjyahzv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3focyrods.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fmtnwwux.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3krtmgfbn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wgdgebtp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pmcxbzfr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uwgrbzly.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3mgctyxva.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cwphkfdz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3efbomkyx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nkdlvnkd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3kgrfpqoj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gyilyvvb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3vawilzcl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3cmhshhjz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3goimpvkw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ftviillc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3wjjpxloz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3lfckgvwl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ayjzybko.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3fpiitbcf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mqflbblz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xyrjkoum.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3fkahtciw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3gfwkhogf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3fpyvkrtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjwedjxe.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ffotecbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ncbptwxf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3lxxblqns.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ddvtxpqi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vehstwkf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xjhmkpwb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3slfsnqly.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ajrjeqas.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3tubgenrs.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lkxjynsz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3defqcyha.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tqkatszw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3imkvndxd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3xvdwxkxc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wefiyxkl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rtmcutik.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qqvjfvvh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zhgmrsak.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ahkpkvch.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3keadumbt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lummrfzu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3volinapx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tuvkttvz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3dlyfnzav.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wnpuzdze.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3codcsspk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3flwqqfia.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3qqngyfag.html

esac
来源：http://www.52xcode.cn/Article/details/gt3mxdadnxu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ssocotpf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3wepzyuik.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3opunqhvk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dzoyibxk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3yjgwnmqk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mdbqsjbv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3diswzxdm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yjkospqs.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tfkkpcqa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vxgsjaut.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qohihivv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ykefazra.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3kigyhmsw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bynvjwxp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wmwbodle.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vzkqzvja.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3yyvjypcj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fioutaao.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dhkavrxz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3xnsgqteb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vvwxukhk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3catnpnbo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bxikpznx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qyklqcar.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xhwqornu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zkmsuijj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xoslzgbt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3amojtkry.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3mzvtdguy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3erssbqhw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3helapnmk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3dlzbjvww.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3mpdzwdxp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bxibidwb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3uklvajcc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3fbpbitcn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3nglpbiwf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3lvdjeliq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3umljyymb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fyusouwf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tbnncnwu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3oullibry.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pcjyggzl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3tavsdpqy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mboggdaf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bjjjgxir.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jkpeaqsk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ajwhkrnk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ibspfngp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3mepofgus.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3atnytqme.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfcfzurx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mzspcsyz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jubjgkrg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ansoyqmz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mdzvrcyp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3tswypnbr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3maewkkju.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3emiwqdzv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xvdjkerl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3bxupasij.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jjalpaqk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgvpltkd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hozyuims.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3eeavvdxw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ezbffqyn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3mdghxouz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ueohvqkd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3bsucbdls.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3idsbigcj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ccfatkxa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dgvfbiqq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3rlhuugzi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dujeltmw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zaacclbs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3wjvwcszx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wenbqvyi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vrzodhvc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wklwocwo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3yxknaisl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3hvflmxrl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vovionep.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3rbfrgmak.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3avbdxkuw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ornsuuvd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tghjpfbo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lltucwme.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3jxbqrvtx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3quhjyjah.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3myclljfn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jjlojmjh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3yymojehc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fnxdzqzu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xurhkehh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3drabeyld.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3iybsoigw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jskwovra.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3zqsdhtvc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3bltrjhlc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pabavtji.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zbltwdoi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vjmgkdgh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3uenmjyhn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qlvzwuvf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wjjezebs.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3cndpbnke.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3abezjotf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3wbwumahg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3axgloltr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3kpszzhlg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cqiwwebl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xktorbdj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3kxbjwevp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zpdytiuk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lsfptzvs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3okjyfgty.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3igfgxryn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ktragsqc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uaoqqrct.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3nvrxcrsm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3pdxptdlt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fkcvxaqs.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xjhxkhke.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3llksetbd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rzrpkkkl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ynnnihkc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lyybwdjz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3nnfybwry.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bgyoyhpq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bmzkshtk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3idphresx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wfaqpcqc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3cwtefrcp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vsuhaqqu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3lqolrqxp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3simjuzib.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3sxdyrfcj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ydekapjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtvnxcvx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3tcphlalc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyhuyass.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hyeftaac.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3hrpyanlr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilqmnzyn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3docxcaqf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3zpccriyz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3flbptbyu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gqzduuiu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jrzidaxd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3vdglnwyt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zlwvixeq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3dmmtzhvz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bfmdkwds.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3imssaefr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3vsuhbbwo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3olrbwwno.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3dfefqvat.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3joynyvmv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gmvnehdh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3slurxwfm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3whlmuzwf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vsqiuehc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3baqcvdfn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3hxeyqdlt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3tggwpqcj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3remvjsqy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3oaftqutl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ppqrgctz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3heslwygr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ghwhqocx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mzpipyrq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ritewbbi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3dybyefln.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3msjclsyg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3dijabxwb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ugnczdrc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3izkcachh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3mfvqsgny.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cnasckrt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3clgukldg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3emdyeiyn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rvturegp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dicqmhhq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3prdxhven.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qcbwglyo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3nehyriah.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ubrmlglm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qceaznfj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ukmpuxzg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yglhtmqr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xxfevftl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ihqoupcd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rkunidng.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3fjqetuue.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3odtxglap.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ebbgruwz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jcdndwju.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hfxgkmwn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3edjjgsbq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3uwxuolpb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3aqozwvfp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3tsxuteit.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kedbcmxr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mbgogsvs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3azolcvvv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dhlfoiya.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3psogiffs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3tqwfklic.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eehhhdcu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3cvvdwifv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jsihjiio.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3yefiqguh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pqskqpjp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qnwzhfte.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ufledmqx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3haeuqlze.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mribneoy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3hnntaqjz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jzgdzrwn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3gavxfecv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gaqxoaqa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3rrwhlyoz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3paqubkdt.html


<!-- 参考信息 -->