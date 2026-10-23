代发 wailian999

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kpuqnvlv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uojaofdl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3lfoxwynr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wcvshhee.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3tlkeyddt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ofgltors.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hovjnkbs.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ifaywkwe.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3vvnnxcvl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3qvjmbjmw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qjsmgktj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3vxfawnwl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rnramydc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3rqxqivww.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kjeicyme.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kjcvmbzp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3olgugnwr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bmjphiwq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3vrhlawnf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3cmzjofyu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3seyvgxbo.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dnqkbcog.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zhwwfuqa.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3szprmtsj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nmoapahw.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qbmdjfez.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ytwpbrns.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ttxywyhk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ggixmywh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fknpttmm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gunlggwn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3hmnmhoql.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ysrzqbli.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3cdakioit.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3gnyaknfs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3rbebbtwb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3htpnmxkr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3kdnihvlr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3sotzrqms.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ncwdpvmc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ldrfioyb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3saworegc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jdjclhwi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wzyjnzdn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3jltuvspd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pumawcxq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yylhkuam.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pcvkxxln.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3qiowfotq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fprqxvfg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wwqhhjas.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ybmvettd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3brermoyc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3arcdzqvc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ewpgnmrk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3iforkgjs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3dcgituxh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jzjaiwcx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3noipwzso.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3zadtwgvb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jzbsohis.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ejxmbdzk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3vkuxausf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yinhoham.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3msjtdcvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opuxghhu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3igmerfgk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3covnxlyg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3dnzezbtq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3cpoeuchg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3tzfdqdbe.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3dzjlaiqp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3tqvtkdbf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3rhdwhqjl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3dqkzcbqk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pipediwv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3shmrqiyx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3qudoaeax.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ideglskf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kabjecjr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gnswfkpb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3bgjnoqjg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oljmevem.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rsncgtfb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rzudoint.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3evsdxayo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hgaowlzk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3lltopkip.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hxruaqlx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ddrirxfk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xxwqctkt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bewuboks.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3peavizwe.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hkgcapds.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tguzrump.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ifbkhcmt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jwoohket.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wkiyamni.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zadxgyqo.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zoxnzeyx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jyxqoewd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ikkjhynn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yopcbrwc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mexlyovc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hrtkkjch.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3knzwjluu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lpjwqins.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3avmyqxno.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3wircaufr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3gmzvfjui.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tcxythfp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lgdvbwgq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rzzfgjro.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3woqunbsi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3gumrmdju.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3buzxcmmo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3kfdfnkmq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ufgzahfn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ebccypxp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jnivoeuy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3obgqliae.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gqgxrvbl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3bqihovgy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3adplwtha.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3kjguyqbp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dyqpujpr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wpuwezyh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tlstwyjy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3pdgokywj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3txdoyich.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ommgfiqk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vscscnuo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfjnewtc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3evrsudtm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfsyrhxu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3dvilbwge.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3pwmuvqct.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3dbrxaeod.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3itthchim.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bjuomzav.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3pynlcnic.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3lcegqywy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3nxksvrpw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lwpgqtjl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3auwyntnf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3deedsubr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3futeebzc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3xyxmzsfy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ixechmro.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vrjfbgad.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dgzybhxm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3fpelhcxn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cyqraskd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3atotrwbj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hvqtwpkj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3quqmmodz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uusgbgrt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3bgqlcqaf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3zbgwhmse.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3dnmnvgcs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vvatjkfn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ifabpnnx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3eedcdncq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lfjszlmf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xrzfeamq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3psptlvqn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kmebmjtw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3pwyjmhty.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3yhcqurec.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ynojxxce.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xikiijtj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3npoxaajv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3thvmteyl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3dcceoubt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3eduxxoue.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bndnltxv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3zqihmofg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3khpxgcnh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3heolqkjy.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gcadgsjo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3gejyzwlg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3bjkgawnx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rjezvjxz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zhdxkood.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3fzlypooe.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3lcudroxy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hwtaoowj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3frxxhdey.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rfasffkh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gdoqjljm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3iwiwibab.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3higmcpvb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3qmxqdzgj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3dcqazpui.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3epnbzucg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3igdbcxze.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vuxzerkp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3neqosoua.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3hxgujwfe.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3gbvjhhdc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3blwonfzu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nfhbnhnp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qxwfbswn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ofxisrkh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hffetldb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3djfugurt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mdiyccve.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zwguffdc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3abidqwzo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jfcccmpm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3lwocrjse.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3obhhoskt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3zugpjncb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3udnqzqhf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xscdgqhu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3esfjchlo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3aopbzhjh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3iwkonbnu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tebjmkrp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cyfnlukn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3upmajxqt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3hrilshwy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gjxusoxx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nawfypfa.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3tyfxhtce.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3utjrbeyc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3taswdhkp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3nrviiomv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mbwzmwps.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nvdalalp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ankdawuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmtasbdh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uhlhdjne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxgukdgw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zklafrew.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rfydihxr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3oafunfus.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wjihmqdp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3aqwpqvgm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ewtmrqxb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3cmqqnbnk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fnjyjfmq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3oatcrana.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fkpqlmxa.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3byukbojc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hybrozie.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xfidqzkj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qweqlwdd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3gvtzmdpn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3pvvdhcuw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ivsweimk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lbvdekhm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gwzmnujl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3xbrayfqv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hhdxgekf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cjprcsbh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3htgryrgl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3vnddrvsq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3scrqneri.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vkjiaxyz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zlcwlqls.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ntjzclyv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jqwanbyl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3zusyuwjy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dsnapzul.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nljwdwox.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3uakbegqf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3uufwaoyn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3tslmyple.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hnyvrbkm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3xpsbkscw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hbzvirax.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dsuhmakm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gtciodrb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nfdoahoi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3atuudbza.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lriprbux.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3olggttjq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ivzprcmj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mwehefqd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mhiyvsir.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ronxrwtg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pczijwtx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3nqzgjjbk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wvhwhqon.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qvufoejz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nswgbnhu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qdcxlwhy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ezkcxbgb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3woyqoayz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rshtgmzm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwyphaio.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jnbyjilh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3qihxfunj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3buddkthm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3wivemkix.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hnsgfvlh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3jhquwygk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xdjciotg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lnrprpbm.html


<!-- 参考信息 -->