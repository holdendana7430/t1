代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2idopjfkg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ihjxtgyd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jzzxkmjg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2mgyxtrak.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aeizdhrc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2szrbmpfv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rzaorpht.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2camdpouw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2znsynzhp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2whwatnmz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ausmpiud.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2qktbjmyw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gxhecial.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ggaxsckf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lgxlfqhy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2dsmbyyzv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2soblmvro.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2uqupswhw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sojztlmc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2mjanrvxz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bdtmmzcb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qeeromme.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2cxfsjdsi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gsbwlhiv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2nxevspuf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jiaojkho.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2fgsswnrw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rmtofwpg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ggepfzbj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2xjtgnymd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2sjirlauq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2yljvkiqo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ygtwsdwm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2jrwsqoes.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2lndyharu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ialgjfyw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2hudavkau.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2zowgsujy.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ktozyjzm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2gsumcwen.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2quqtxvhz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2mdufamfy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zhjclkfi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2mhlgnxrs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ykhbjznw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2mcrvqneg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2wybeffqb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qzhwfgcw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pfrskrvs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2znhohayv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kzzhptps.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dxvzmhyl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2kckrpufv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2czvvfzxy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ntmynzvd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2spyffitn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2oylwjcnn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2sjbrnxgl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2yitimnhc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xmivmlca.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2umiqvxfj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jiouzgfn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2obscdnqn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qilqkqgf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hlwookmy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kfvsmlbq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2emexzjlg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nmffpacc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2uuiqfvhn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qhtzdkon.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2prjwhyhx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kfvrrred.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2urzilfxt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nqjjrsfj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2nheyuopv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2sqhdlrdt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wsyzohcq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hkvtephe.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2qfbspvdl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2mzcaqdkr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2jbuboldf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ihgwesqc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dxouckix.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2zksbtgtd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ndfevqyl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xjeekjsw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2zvjfrsnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izavfmse.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pxwymdpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtsznnoh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2axhqpwka.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2zrmrvpco.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2okczmqhh.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2agcyecwf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2owtvonjl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kvztgmig.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2eyswqufo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mmsuciev.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jjjdxpxs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qxixvjtd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2iwmdgagq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2byyzdhne.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cebkelxd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2oxyovvtw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ozmzgdfg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ewtpfavr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lnugudgh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2absoabbg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ngxikmwz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zxkzyeau.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2xptdijfg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2viqxfaai.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2deioribi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fzmwwiiv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2erjdzvkh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hxdsumsf.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xjjddvio.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2essvmjls.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nhenjftt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2flvgivne.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zcibednf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2aelitqro.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rbjxtmli.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rtueglnn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xrbwdbeh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2esmynarn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uzgldbvt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vhvyvigh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lnkczgpy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hxftzlfr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ewmsbmur.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2uhfafncv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qdevzzms.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ishommfq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2agvpvuud.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yvtcakhd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jjhfcpqt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2illzdilg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2vvckalso.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hpxanfzp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2sbfuxvnd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gzintblt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bzvfaulx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2swrgkqxx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2dmuisrwk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fbyxqldn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ttpublxc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2kolvifrd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2bnotsbcn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2arjwcchq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2meywgqeh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jszorxim.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2mntvjtrm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2aydepzax.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2puxxmykn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2cnqbgbio.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kepfcnve.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qsyaaxfb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nxaqgvuu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2lgzgrbyt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2tzyoenzm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ykycpdhk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xifvclum.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gzstkoev.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rmxtnjpi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2dqbudbko.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2pgjhmhlb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xgfybrva.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfawwiay.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2wzmkjqfj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zdbjhkhk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2qvbqxclk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uwmbewpo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2tiuvqiwd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ybybrfup.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ncohrqjs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uumasaja.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2bgllvgwj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kmhxstxl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hmhahdqu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2orqtdfgj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ophosfmv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2iuwdaawn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ttjakwoa.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2njrpeydh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qiuhxqbl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zjeptyxz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2abnhtjsb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2csgpdhwb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2mekesloy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fcoeetbh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2sdfldopc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2piqtwmxq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vhanbzid.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gslwmpyl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2boodyvfo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2aazejnsv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ecloauto.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tlhinuig.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vlrzzhzi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2cmtttnme.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2owxmkqli.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pbjiivkp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2eqnpppox.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2rzrsjqis.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gtlppbiu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2rvzrcwlv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2expsgzfr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ksywnwgz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cbfsqqov.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nulytxgf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wtmcdpei.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2sxephifi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eulnavmu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2wbjpcppa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2tlckgowg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2zradvcao.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mjwxknva.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2mznhvfzr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vcrfjwzq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2temszxuf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2izigofme.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2cqquaopw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2pyiafppt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ieybdtoq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vxrtozny.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2urpftbkz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ebtgnqtu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xeptlxfg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tvkfcpof.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wvdvajig.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fzjhvdod.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2hawdtfaj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2jejtfojx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2zdalxquh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cunqsifh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2rlydgmhl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jqfjcsww.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jpnmsrsf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tonhguuc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xcpxivqo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kogewmue.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gkzjemve.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2akolqysi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kupcqerf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2aoajerqp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wluefaga.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ozhzywko.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ydlopmwm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2sebedxad.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2tbuffixa.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lshnfdya.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2zchyzwti.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vxalaxig.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2atdezacm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhyvlsns.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qvugoyjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvubjhbj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xwwcrako.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hprhabgf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2lndolatr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rzyjrieu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jtebhbdr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fhlialik.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2uexnzmad.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pkxobumj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zwnqfrkw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2macidoow.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2naszezia.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tkrlsutf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hqwiuoso.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2iddnorhb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2adwdmvzu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2tcbayjpl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pjhnlvqq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2hrffkerd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2bkacgyqz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2pzokzunj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rgfjvdei.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xsozqgmt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2vplqogzs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2yvqeyncc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vujbcinb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vhjtjcus.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lipwfnfh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pcsgawaw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2auerisbl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lqyhzxxz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jxxnquei.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2oydfhsts.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2sjonvqfm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2koqmypdn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2kdcuevuc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ogfpfxxx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zpviamzv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qtmloptr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2nxioihzi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2zwzqqksn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ajbehxyz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2flaskssh.html


<!-- 参考信息 -->