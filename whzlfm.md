代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qnscjpmw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qkhmbmtf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hrkwcmsg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2synrfgkj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mtgxrmbq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2maylmrdg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gsjkvvpn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2htcbwzwi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2retjshqc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2juzojllz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2tienlxiz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2adxsurjb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jvnzutpc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gztrrzkc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hohcdqgq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fpzhycam.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2blemypsf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2yjeqzvld.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ytehpfgu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2bcvkhmqr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wrgjgguh.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jqfzcsvk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2kcbbnadf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2domlilrn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2vlhsnczy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2kxjdoiwp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2eqesnlqp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tiykvkcu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2uznbrnxn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xefayvdy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qbnzdolh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2xqkwnujz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2dzhpjawf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qycktqvb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2hxrlmzxd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xdielrxp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ifjhhqit.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fnpkocur.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2aqgvdkrl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2fugcgzxu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2onxekekh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ddvztpxr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jetetoxu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rffoihfp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2nlfiyeug.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zkkdilfx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ukpgvixg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mgkkuxlh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vabyvnzk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zcwroipi.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yfoynbzr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2josujhej.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2tjrosxxd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2udvpkksf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pzpjefsf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jhicnypr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2arpdfgpq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2omgeexln.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ovrxqfrp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ecmfrjdv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2bxwwnncq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hillnvwj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hcihviwp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rqtyfixn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jqtcniqq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ugvrdyuh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2vgvqqbgu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ipnwyrkn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2idxelnwy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dboyianz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mmmnwkgd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2hfitwgbl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dgrlerhc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2uokrjqmi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2owodpkjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gslnuywi.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2fjvfoddg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmrvlpxf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2fywujuzn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2djnjycop.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2maliebxb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zkedwwys.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2telxyjuy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2lxqayvvm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2pintyoko.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2qgkohsqm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2hisixoeq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2bwfuwhru.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xkvvligd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zzfejqit.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2eubfzpbf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufddfjep.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vypzmfpu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ohcolseg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2emhouiqw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ebohajat.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dhmntzht.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mnraxwyn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ddzsaabf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2nsdcantc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2hkjwrqma.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wbudmavj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2aftzoxuk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ozjmygbd.html

esac
来源：http://www.52xcode.cn/Article/details/gt2thlncgmc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bdgpvfyd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dqytytpr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xjytinzj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2utmshill.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2nphurrym.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cbxaeluz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2duyiowfk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xbkogxam.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wxajkzzz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yyxjqafi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nmogfsco.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jozlpome.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2wqqqbfss.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2imiormqg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ndujeyvw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2kgxrffpa.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ilyyabfw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xnxxijen.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rujhnpjd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2upjftoql.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2manmedbt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qhkpbsbh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jnxyjnuu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zatedrml.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vkzaacwp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dvfrzptl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hjxgqzoo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ghfeoemb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2mqkttmaq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2osuhoisv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2tjuwirhn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2chsbpsju.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2aiayhgct.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2xzabprxl.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wxttvxsd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2rzpkgyqh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pznwcrkz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2klzuzexs.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2byniqtwk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pkjfiuvq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jwgndbqc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hibwyesi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mcgqpmlc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2tvlvtast.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2mvdypvpe.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qgrklcbh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2bnmkikfs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2aplcxkfu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2kchbhmkt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2alleaslj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2jduzzayf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2apfwyshn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2glmitwuy.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2samztxja.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2cymxhifa.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jiytffvk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2eluzludl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rbxtltnl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2tqndqtbu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fcaapcma.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2aaegbfia.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2xxufjrfj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2luqvaqxb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bjezjsvp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2wfnwzwbb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jlzigwui.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vjwhjapx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rumpygfe.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2uhcsirfl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mfekuxhp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zjdrlcov.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rboasphy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bzquoxjm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gnrtheut.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2prnzxfmj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2yyhrtujr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ifgruayt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2orxbmkul.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ykxglfxf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2kculoyqb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2gkgstfqk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2patloqjv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2oqkvrgun.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2pwuzvpsr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2wlyuhxgr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vdctkbfv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ttxpwuso.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2mmslzlcy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cddseodr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2eziltcsx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2nufxqakp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2gkajztvp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2eelktaog.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2chfmgbbk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kedchvzk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ejpbusxr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fivlctut.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2nsloyvxo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2goyoxadh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bhulieqb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2dmbmnpgo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2uepfdaha.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hgpcfgvx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pwulmcin.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nqtosqmh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2lofbeevx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2msvywggm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2yosvmefv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2eyefkezr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2txbtfuki.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2xtortdnt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2sudqkvis.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ygcxbmjw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2mkxhvldx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2dhmmtzlr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2urkecqbq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2cuwxcmjr.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2otobrexd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2szcmjtoe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2boicwnad.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2cazdgtnd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xxemoine.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2pevmtoar.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2pwrngbhx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vrvophji.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vqcojrkd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nkyasted.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zrrebdni.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2eqegaoep.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2iisjaxbv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xwgloxpb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vpefzqap.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2avdzbyjl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gfpgljmj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ytqtybus.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tjvgrzud.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nsifnveu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2dubvmisp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnxeacum.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pstvbjqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbksmhkh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zlbpbbqg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2xqbhfsqf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2kdrwlizi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sduhbsfo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rjkhskub.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2nkratqtw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2exehrhbx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2qidojbvl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2smwllvno.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yzxhegth.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2uuxhcgjh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oehnxduc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2fdfydkjn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vdcezzoe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2iiatiumz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mevkxozr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2kbdokqxn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2odegqdxh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jduwifsw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2qvanwtvh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2phjzvvcf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cfcsfhpa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nuwrqcos.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2yhycqvpz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2eatxsnko.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2htenrnfs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dnrhjxkd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2uzwlakir.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2doucfmit.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rkasaowd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2fxwtudyv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vkyttvtv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2sppmsxxu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qcqcfyzm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bkuneokk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oaejihka.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ssahfqky.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gvqbwyae.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2nugzuieo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pjufkpfh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fdfagmni.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kjgjmqqn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2iphkkjct.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2nyjvjhea.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2nidfdmjn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qqhxejyd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2wsgeedio.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dqdmhbbh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nrzymmfi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vujdmbit.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2olizxsgi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gvjxazji.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2sausqvgs.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2bgeeaehp.html


<!-- 参考信息 -->