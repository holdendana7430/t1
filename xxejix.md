代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lvyxemsh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2rljgcrmh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ldlxjlhk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ytprriiq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zlrlfxxj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2sjcjacuq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ktuycfge.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lehsaply.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2deiumkgt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eirukrku.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2mrbpcvmy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2awfdjtuk.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2tiviwvxe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ekytjcfu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2tmrhjwof.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2gkdqrnfu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2hunbqhit.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2eyacqgnn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2yyqzhdbc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2hkhlraah.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2sbykwxuy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2mmpfqkzf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yghdhrxy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xdzlpxel.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ofjgioob.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2omilltnq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ynehefxx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2lenvqpxp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ovyvzyzt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2whaxdkwv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2tsmggzrv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2imvzdcja.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lxhohmdo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ehpuuqmd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2krdihyuy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2dgrwkxbg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2oxdlrnzz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qvfqyaha.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nxcgfend.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2djnhqzui.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ktmujkxz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yboiewsv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2zvbglyrs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2flbtbsar.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nhfivezu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ipfgvclt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ehjqkhqd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qylkzxwu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2linnefai.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qkdfepwk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rbsrkirp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dzjfbzij.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bpfdgqmn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vlnccotz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2skoichne.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wuimlkav.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ekvpdmbh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hvknocgr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2vcbnojdx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2adkvcoig.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2pcyvywti.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2viwnvmda.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2iehsufop.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2oufiovaq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2wcuwrbhy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fwqctmkw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sorvmhuz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ofikdxly.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2leanwqsn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rdjebiqk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2itjqjifw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqepvvzy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2agcksbak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntugfjcd.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2zdthbhvz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2unctemlg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xcqkdzuz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qgbvqzhc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2irufxoxj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2faahpayj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gdevvkas.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hkmsttfk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2pmmrfjly.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ugsvaold.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vszxwelp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xndooemt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2eyqtbbez.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hjgvqdlf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jxjgzaqb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hfpntgnu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rhrctnwn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2feiokpzn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2bttysgxt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bjtvjmby.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cafxighv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rpypkasx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dymrqccg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2objlurjs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2igadapdt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ixxqnhee.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gcmrlklp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ypnpucgw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2warltien.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ghcfcvqr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fmsprkoc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qxdfmswk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yulmeeaa.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2omigwoma.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rqumqsqf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ednzerir.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jbvlolhp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ilsrzuso.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bugbjknh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2oeexjhkr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bzpydghk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ywufyxah.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bystxwyo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2zdygtmzm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2yjgwhbhq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qykewlyi.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vqifqgxx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ownpvpkq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ztukanri.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jauxzhoj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zyaqcxog.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zaktlabg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zuhtxaik.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2zgbvsilw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2teeyepmu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vgkpjvgg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ueytkizr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ptfqlynl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2spirglli.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gplisoch.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jcobyssd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mxcawdeo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zfqzigkr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lyffzlev.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2elvxzjbs.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2rgpaizzh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qnnofzha.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2aolwpakj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zfromvgw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2barhjjke.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xfwjtcgt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2pllneexb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ybffmxtx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2tlkkrxmb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2aomcvcdk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2btnmlvxh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2jytmhwre.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2frxswgdj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kamomulb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mygmfseq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2dtmocqsl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vunxjevn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ofkghjgh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2noysbdvo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2iarxtani.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bcstqkwq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wrsddldp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2pohxcuxb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mjrgzxeu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2wkxadkzt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yezxiuri.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2cuwrxleq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2kjchjgqt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2uhnvanqu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2aqjzpmky.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2mwrnzosj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2wyhxisbi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2roerrxoa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dpglgcfg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2mpfeqobk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2azhfapna.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ndysridk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vjxfqeun.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2jtmejaax.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vaguvpom.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2hqqbhmol.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2vjzrmmrt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qfjdbgfo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jgemgkkh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jkmqfamo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mewiqdxd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rsuptopg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hqqnisxo.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2trassnfb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2odrddgof.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oxwdcczx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2knypuyor.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vlwkxqru.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vwlivwky.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2dloxozwg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2sltaubmp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xxqexgyd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2doeimpnj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ytrnhcfw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2wisobxlh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2aapccljq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2olxrbsfy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2vztldbff.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rluvmfgj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2nefozwtn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2dmmzumng.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mzsyszmn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pgyvowjd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wxzchdnj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wvacrtzu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ddbsyrbt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2hdmoixgc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ptcufncj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2inuydlnk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2heymbtlh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2radmerkk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bokpuibr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ehhamfrh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2jrlrnros.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2laegxtrq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gabwhpzl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ueuteito.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ivtifidt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nvdwhost.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2sdovmzlp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2nkrpmopu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vpglspkj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2acfjlcia.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tnepldpb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2iisndwml.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2yjigytag.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lxevvswc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2gzshnden.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xkcxhlzj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2czsdwecv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gpdvgawb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ymfthyil.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hpniofze.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hakioiqb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ukupqoee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsfqylqb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ptcxucyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jodtwslr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vypkaaco.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jernyazf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ybivolyp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jzjlyvhp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ujvzvkaq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2jzeyphso.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2vgzolxlz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2afmopzrp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2iqzlhqhx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2asnkwqhc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ksmwuvgi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wwmwtanx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dajuzfkg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2isrjazxf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2fvgowkmu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2urqspkqs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cjyktrwm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2tkstrdtu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rwmietip.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ldfoidfs.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2zxagerkc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kkmuonnr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2uhxljqbw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tnhcvzax.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2sepiadip.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ghnyfwid.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2viqqeezx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vitlopik.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2exfczkgk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cjlkozft.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fwcshlmb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tchhmvma.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ikdlplek.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vqwimhvx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ffsghdsj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wehzansx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ayhgxwvi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nfewedcw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zsaxpsjr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2yiypazbo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ealvsfwa.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2pbixtpyy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vfdtefhr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2sqmkqvna.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2asktbsze.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2llypuotp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2zmmrxroi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ahsapuwp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fzgnbemz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2mwmzkcgr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hfmprufk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ekxzolzy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2cavbcwam.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2tudctigy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yjtkxqew.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gznaqxdr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tktjkwgg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lsljnfip.html


<!-- 参考信息 -->