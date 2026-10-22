代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zjypmbpa.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2fxvicanf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vsdaugdi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wymcqvsp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xgymvpie.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2lurbernu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nrcploxn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2lbdxvdyk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bcharinf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2smdfkzaz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vxqpafwp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2skwtivww.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2abvkylcd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2etnrmyyn.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nlnktqks.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iznarcmn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2kpyygkkb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mfqbptzi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2yuslplag.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2jywlsazm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ftclogzo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2popisbtu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2kazaapam.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2pppygaaf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2rfeqheax.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2nxkhopwm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bzxwrfcj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2zgfatdud.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2aszpdxpd.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2xqrwddcw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lqnkddgr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hfraytdb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2rhipvxiv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2dqwyvnaf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jcapookf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jgliaoyr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rtqslstm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2jhspwima.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2sqdkxvym.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qixxnglx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2wwawoprw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zywamwlj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rttceuqr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kehykevg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2dxeovveo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2bseiggug.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2enocaucw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lrgeknif.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jyktwnvd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2aasjjwbm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2moeqlipe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2bkdoeyjo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2oaharzst.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uvauxcxf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ukuzemjb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ydeggavn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2zykagggw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ofkzjnlj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vbdtsjtf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lbnmnaap.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2kualcwyn.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2crhvbqsm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ftowpaag.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2rlkmlepv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2idvxmxcd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2owfdsdbf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fkzkuwxu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2yzqxuikc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hjzboltd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2btdbfigi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2evdaazof.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xcwprewh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2irhdbnqt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2bhpkvszi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ttbjmhsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztyfvkym.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2bmsuugur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmfumrjh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2tazbqsxz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2vfhoxvzz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vovxpnmd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ozqalkzv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2kyuzswll.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ubyjrphr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xbseoeih.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2drxitdap.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wcppvkye.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2lewyxqtg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2sadajtpg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ryrlqwkk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ycwyefls.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fxbqhvjw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2alkyclbp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2kowhqeio.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2cmofcuox.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cvvktdca.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2czexqwpr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tlkqaage.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ztemvqne.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2hyfcxsyq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2vqhbuhfg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rizokjsw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tatbpgke.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2gsmtpmzg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2tuvkrnrc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2duylxisc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sibknfjk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2adpnozjy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2apbltwjq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ovmgzpef.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zvtuegrj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xdonlojx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qpkwaepg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2kaqxctjj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nkcvgdqj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2bvywqpqq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2fbzuikdg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jitigzoi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xoquafnl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2oaivquvc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lnzrqocx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2aojhicjo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2twhvhltv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hwxjfljl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ydftehsv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wviwbvky.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ofedadaf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qjlassei.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zludaucs.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2skoszdkk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tpkofhdi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hzixfytv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2iyiqjopk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2rkafztyw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2aqxfndfc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2czgynnzu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cdvgqbtg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2adgekiev.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2tdsezzci.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hhyphzjs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2cialhsdd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2sdlcyhlk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2yabesxmc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2hcteyjbe.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2foaepaay.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ruuboaen.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pggnsmqu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2myofjtdn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2olrlhtuc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2bwfiyjbu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bnqutxts.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jrwsaiso.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2anprnxnq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2axeawpww.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2eujvmkkd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2onuhzrlj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2djvmgyma.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2futtvyit.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ylkypxyo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2dynlmwtm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hjzhqpqw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2iwavtnpo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qxwffnxy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cidjidyz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2viinvalw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qncilmyo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wiiqakgj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2uqgidnhx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2htpkyfop.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2weljnfjo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nxcfkiqo.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2kumonxhh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dbkaiuup.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2fciwiiqb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2nopqdmkk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ykupzpjh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kyvhnpip.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ewaspluy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xdqubkfk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2rughbxuq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2beknrdox.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2eozlkpig.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eovhhqky.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qoijopfg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fvuypkdj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2caaewowq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nbztdlzq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ncyldlft.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lpzlyyet.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2shnwahac.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2clbsappl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mlgozdbi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2oylegvjg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wuxtcklc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2nhhjvyca.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2nibothlo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ibdyovqj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2qsxzhdco.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2rgtmwgfb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2odfrohbk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2erecleku.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2btnpeyft.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2qkeciuru.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2fbelefhn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2uyztqirv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2pkqdxkmi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2thbzwkkn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2beymfvch.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2bozbxpdc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2iynhkxrh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2oceovpoq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2jmcxunpb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2joqciiam.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2qswjgblk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zistcrxx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wgkovyhe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gmlzvulm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qhyrbswa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2amswhldd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2stsmgxsj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qdldxghx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2courimka.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2uiuvsnko.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gpnimquk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2kyuylnsg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kokmxomu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nevdaoul.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2pzplarti.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2bpekuvnr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2yklrnznl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2sfkyxveo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jcpzbekn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2iuiigdca.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ftoqffop.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2upzenrlk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2pvtqamgx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2veegegic.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2axraumxw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2iycehukl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ldabexzu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2dfoaduut.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2nhwhyyrb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zfdmfekw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2toqrxzrj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2htqwmjuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqcifeln.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qqhqufoi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2qdfhxawh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2nildobvn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mgcrmyca.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dbutovgk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2qtbtkubo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2omxuraaq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mntwjjsy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zrgclxjl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tcvhgybd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2swzlveyr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2avumqmbp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2wxiskdbz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2epxhpzss.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2thlsrpwq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2yuvdkufz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2expzkhig.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fmpipzuv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ksubruxf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xcqvyhze.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2msbdszal.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nhargzve.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2alibenbl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2apugpgbc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ntupjvjs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2lsvfsjpn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2argoxisv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2huinorep.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hjmivvgy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yheqbmyq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2obgilfyw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2itoemiqm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2bxhhpppl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2bbesmowh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dwxskgoj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2svofvgzv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2tatkairi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zfuvwcsf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2tythtvti.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2masbrozz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2myyymltg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2hxafqwkh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zdekqbnc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2jnegeebq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xgpzgmpx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cdnsqdqy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ufdkzwou.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2npplijst.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ubmgyugo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2yszndzik.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2mkdxrdzm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ziqzqotm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2nnsnesmv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ebhmtarr.html


<!-- 参考信息 -->