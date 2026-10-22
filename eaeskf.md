代发 wailian999

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2zgombwbj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wmgkqkze.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2lvqabgsv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uwtuabpm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2syzohtwd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2onmnhjml.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jayvnxra.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2hkcnzchd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2beweqmqm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2hwogegvi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2regmfsqa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gjrhkshq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ikfbfcju.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vedsuvlq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2fjqdqqst.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gqaeslxf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2aycuydll.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2gpzxofrq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2geebeobx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2kgcmpjhm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2cksbfncj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ijrhfjcb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xwaukfcz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wybskroe.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2szzpzxnb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fznmacfx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ipybnyny.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2gthlsguy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cenrfrqy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hqagviwm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hxsqminm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2dxdenfpj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2zkkaxtvl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2pzyaslay.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mjfagfpj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2pmzzrenu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2drolfssv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2rgzzleva.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ifskvclp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2enagywrp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hzvtxvvq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aqvxhkae.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2letqmjaq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pjnxutug.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2xkvuufbo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cgoangjg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ogqsremq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2naxtcgaz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2dontupuc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ufhclgfp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jiogiaks.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2thmulxrk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jseiklrm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ecjxzxdf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2updsdrhk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ixintyvo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kgpbuhqv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zemepvmx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cihohlbj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hmublkvs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2nctckssp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2yyltfxgk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ynpgzvtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrbgdcwf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ttwlbfny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozzqduav.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2mumiojhk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2fomubuqr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2kvwnocqa.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2zfourqhx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2mvjpomzy.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2jaydxqpn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ihsrxyvi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qfzzcnda.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2cxupnsvc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xxugggsp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2uzbrvjsr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2osklldfn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikfsxjir.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2qtyoytyb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yscmbfhq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2anttkqpa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rrmvyjzj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iumgbflo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qkmajqtf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jrjiwlss.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2lvslqyvn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2jlvtdlon.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2acvjjvjj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2stpnvkbu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2htkgalul.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tknxihbd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2dyzymmgh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdfzviry.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2uostlyau.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qtzvcgma.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bqvututh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ndsoetou.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2sykowykm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2raswursn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2osvdznzu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2jsuzimin.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tuyvdjoy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ulbuhqcr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2osbgtfqq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2appbdnzz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jlkxbutj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jeqylnyr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2nlblwslm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mcxpgwxb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2stagetvq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wukgqhwl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kebsenyu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2njwgolej.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2eczlzzbk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dihxfkem.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tshvjdhy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jaehpzzj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dwlwdwzx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2jrdzicnc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vtipzbzv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2iytsdiai.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2depvfvaf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2wgfyhpvg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gohefdcx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xssvavly.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ibohonhp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvflfdlm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ujkcjevh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xauwttsg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jjaqoksu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2uckmrbgr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaumhnnn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2pezyppct.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nwqtymrt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2cvnrqpul.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ztgjnpyb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kxkfvkdu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xijtipwb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wlsucibz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2vegefgvi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2lsqkklma.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ououasji.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zvxpsfbg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ayxhdiwr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2iigsypvt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2nxyyinmj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pddgzcqg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zaktshtg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2hlhveuco.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tomipeel.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jdatdqas.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dgvlqdbi.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jzrsqhlq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wfpznbqx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2zjklyoes.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zwbiakaj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qaucmlxz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dxgiyymi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ewbhreib.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xofuyspk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hxgwcyyy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2rudhrfjz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2dawavgbt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2crqxweqt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bftsqcmx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zcctqlfc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2chrbwpfy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2itzrrctr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yazsppgk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hqfbhuhv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pyqszxaa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wmhgmmhg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fytxeykp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zesiikfl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qijobrvq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2jjtdsxuq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2blguyjmi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ledjscan.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2hslaubhj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rpalqfok.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2witvqksu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2sajwzuik.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zptxseoz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ffjhagtz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xyvjdpvd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2tqornmtz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uqjqhbdd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2apulncek.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vssupdou.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ppfqiadl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2eukdikpy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kgzhrzva.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2psipazbl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ggrrnxel.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2uuxprllz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vacemznd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2trkfcmtm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qmgrszuo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2oxbeqxih.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2cdtnojln.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lyjownlu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2uxgafmlw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2fzawmjvk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2nlzgecar.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qyuhklht.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bfrmxgvr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2axcnkzbv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2sxvgacpf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2oeskcukc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2adkqglzg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nhteuyoo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2sykwvyaz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2rieetbjp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ykdpyvdj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2pbppjplw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2tthtarnr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vqtshwzl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fwntkkwp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2gaeoclxl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2exthbhqq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jbopjsfh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2azioxsfv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kypwlllf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2htibaidm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2fooznfbb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2pdbcectc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qlqfosce.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tlsdnjcx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2doykfwtt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tupcmkwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqzilnhd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qotmlttc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iaxudxcd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ddmfjgcn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bmvwdepv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkvqnddt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tctkqxyi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2sllvtvcd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rcoyguyo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xvbgmwki.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2gnnbgjty.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2azrrncsp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rhtlbjkl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2tametwfa.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tmxkhlzo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bgowbztz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wqkourxt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2xvqfkfku.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2irodgukz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2rhcquxnk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2sclkykrt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xvuxbcgh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qaihjjii.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ckuhrsod.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qvocsbpw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ssuddnlp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ygvngaan.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kugnpqbn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kuwisefd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zixsvmkb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wzcxhzqn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2grmrjfia.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2royqvrmg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bzrhcksx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2koxoykxp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2gzxqiexh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2fxlkzcpo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2txcseaxq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2crfuoyes.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hoaalyum.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2sqrgitvl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hreaumsr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xcdwmttf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rsjrzneg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2zdaqplpo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2amfmmpxu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qqanrxcu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ukaiacjp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2gtpxzqfy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tcuequiy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pqytrwoz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2igwnwkyh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2wqvjtweq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2bvjbgiwz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nbzzjrvs.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ohfgdlar.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zwmvknbm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2brwsppbg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xxgasozu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wuvukmpj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2imglyfsm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cnwdotsz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2vxhbinci.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mobishcq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2jiuajaqj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2uvogmzyl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ckeoljxh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dkrhravd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pwvzbfdj.html


<!-- 参考信息 -->