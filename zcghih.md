代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kozhkebz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2woigoako.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2jgcfxapc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2slyvvmuj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2innjvbhu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2vlepyube.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xmqrqqta.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2mzgpnthy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dnrelhnr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vbyzwivh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2edqiychf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ojvepxlg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aeozapav.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2tccrabit.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2vnneyvmw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2obcnzixv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2fqfmaarm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tejuotww.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2yacpviyp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2daloaysp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2sllufndp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2kbwslprs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zupuwqjq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ulqxkjcg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2jvqxezhr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2errbkoec.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2hiwcztrq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xrhhwjuu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hcyqohnt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2lxpoodnb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2lckwevtb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dqztfxsi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2kgtjkstf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2dybbykpy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2uunsilom.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wtihkdma.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zpujqjab.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2jaeqliii.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mmmubiyk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2pmdsreej.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2usrdgbwd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2jxgceqhh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qpvpdxki.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ypvlktyr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nzmxkhjr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ofrfvrea.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mrthavsv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2fsnkgine.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2lkxszusr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2bkhfzkpk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2cnzulwil.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2vfyrabvq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cjsndmhy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2keqlorae.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wudnkhdc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kztizvlb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2uydrpqom.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cswcdmdu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hjhqpdez.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mdftuxkt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2aclasmsh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xgzustzz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pizrvxzy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2btpoercf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2akvfyhvg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nvmtjbdi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2swwhebyg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2tfcrnxux.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hivattxd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2eiioerbb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vkncnxhs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2slfcwjio.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2iultfuwz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2mcletctj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gatgxmre.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dnfrtqpd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2gdozfoky.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2yjbwavag.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vbewgoyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvwrzcpr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rcjszlfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jydirghy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vgrklivw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2tphaufim.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2nfptegoi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2fekzluhm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ylkczprm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2krpupthh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2gbdwgcuq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mhdnmteu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2tzanwyhx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2qjsjcfnx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ewtsyqod.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2seiiygtv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nekulepw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyfqxdqu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2uqjcdyej.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qratliku.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vdscppii.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xrzwzsvr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fbvsazad.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mgpjfgbz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vsmeuxzg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ghxawsih.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ctcebhgq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vkqavkrg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ixrknxcb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kjdonvyh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2djjpwrte.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2kusrgrjf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gfiwtvwb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2iapikekr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2htqxmvot.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bsxvslml.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2czzxflsr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ncnvqpyb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ahoweldd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xrwjeepk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wdnvlmmr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2wpxihlna.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gtqdtukm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vlaapxzi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ofzyvpbk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2knyqjaan.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ychyqctd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jrwqpoly.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2etpbxyrg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fdhuacax.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2mbvysecz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xgqddwgq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2wsvewcgq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2giqinhin.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2rlsmoecd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2arlfzieg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vhrmqkem.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ixawxjvu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2cegqweyg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2kccghoqe.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xssnweof.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tumvjyev.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yexzbafd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2sjzsuzau.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xsqeetwv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jilsuzld.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2npsmuaih.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xlfadmle.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2vtqhkbqs.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vrulgint.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2cwtrwqdj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2bwkriddl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uqkjtzcb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2opchsfzf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2woorsloa.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2cqamiiua.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ffcpfooq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ovlwvwrl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2plhnahci.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vlbtgnpe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ymabpehn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wdtkvimm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kizndhsv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2fizooiwb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ifusmfxp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xuyjcwcs.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xviegkgh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ppviwkdc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ikacbofa.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2bqkyztaa.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ybscecpt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2axdzuknh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qmwuvhrr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2uatqzuoc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2oekeonrl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2gbvgwham.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cdkqqyjm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ipkgplxs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2tpnpcyvi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2dqjxwecv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2bvwlmrbr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2sgwmtojr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2isakawsn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ikkrgwvx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ydrafiqu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2yjghrgui.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2xoasqdqr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ytwcbjxj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ojxrhkek.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jdsnqvnx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hbaneonu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2hphxptmd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2snqfdbtk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ywfxmcyx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ayctdgjh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ahehehud.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ljmtimrk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xhdcxcdu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2iddoazld.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cbocbrnq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jfjkgklg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2fxrftljg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2tqebzexe.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrnwejyv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2tjbnypqz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dctmnvcs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2vjouikix.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2steqeycy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2likullce.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2rapyziho.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2lmwhqowu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2zvdruugi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ninwlqmj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qejowebj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ubxrupta.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ziaffzpc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rfufyidi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yhvihdfq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ddpoaijn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mkaignnz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2sdcafvyj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2yppyogns.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vapbckwc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2nhwiougj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hrntmdfj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2twknlzja.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2jvevzthd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2nkilmmnj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2rjbdvnnk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qzpmbbtf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cmobtybf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zjeousir.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2owulrsin.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rccthnic.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2nwohgufy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ivzzftxb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2douxalyw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2yoxxneie.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2gxwczsyv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ccaoftmx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xiqoaenu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ygvkkhtf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xtkipnrz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dsqwgjhp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jzxmrgsr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ntzrnhgx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2uehykkat.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bfppaklg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2htjdaivn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zyuuahmk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hgzaifsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvgogqvt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pxenreex.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2qdwsxpgp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzomtlvv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2whlbzlcn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nbqlbmpi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wlugvjdb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2tvwgmnvc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bujjeyub.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zjnmqzid.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ifwfnxzw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnovpxub.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wtrgsggg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hvdfrzgq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2unqtnfct.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dqpupkqu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2oxkzkqct.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2phobzcrb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kipywrar.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2yqmdgzkb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xwxrixjj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2epkovxcj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ilnpquqc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xgwqsgpb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2lwpvhjon.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2flzvcjnv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kkqzsvzg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lzstalbv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2lcxhkuki.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2aoimgxfu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2belxtlst.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2eafmypsq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gxmcrkue.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2zgsoouod.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2xlnbeiet.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gdudwnec.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pwredsdd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2cvxtutxy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hzzqltss.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2tykbioit.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xmaglsto.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yffdixbz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xrbzensg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rwnewzow.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ndyqkkfh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zndpmnaz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bfvtyftl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2elllmjgh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2opwecubn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2siktenpx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gxduqviu.html


<!-- 参考信息 -->