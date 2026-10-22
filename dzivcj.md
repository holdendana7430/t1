代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cjfhmktb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ypaezlpt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2wbumxwer.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eqhcwatg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2roxkpbrx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ussgwosu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2hiubbopp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ynhyxomo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2krfqmzxi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2pxvclwif.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hjjpqvhu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hxlodvkh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2wiuhnoqz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2dbqogwvg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2idfljicy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2capllcfi.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2rjotbths.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2xaxyqshz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2kynfmhrl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2dqpckchn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ydytavoj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2jzkgefku.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2trasqxkw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fimysphn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2fnrmhxbw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2pvwwbiba.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2wkljjpch.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2gshdnjqj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2huwdiadv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2gexdxqxc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2oudboger.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2wuroocvj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zogtzvov.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2inkybsbt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zyamqetz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2eyzzajbu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2efssowid.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2vwekdawc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2xatnhoee.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nntzzgbt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2srhlsegl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2pltygchb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nzhahxqi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2urxzheuw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2uvlfhpng.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hdwbitsp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ohcmntvo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gusboajf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2itkkukmn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fpigatdr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qcsaflsq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pdjwdnfp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2rclijkfk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ubwyycyc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ennzhrum.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2tuvzlgem.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qrbxawhs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2pkravvox.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2iiqderhl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hgqcltqu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2sdrlofnq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fhrwggxe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2trzommtq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2awtgewyz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2srfncnjh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ylztusue.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jbbsyybd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2riqkigbn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2eaafysbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umgniiln.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ibskzmwq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2amiikbgk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tcdcnlok.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2gtfkbuqt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2nrompoxd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fhrqbbgk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2oxjascsk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2bevdvfgl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2heefdvwd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2wmppqmeo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2mbzalgbd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jmxnaxjj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2weldinco.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2iywaemxo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dwucnxeh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pflasqqq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vjvuqwpm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2buqcpobs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ykipqool.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mpvjcnqc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ceeuksos.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fdfkupqu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2jkbnlfov.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tvtepftx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2duopyksg.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ffwbumbh.html

esac
来源：http://www.52xcode.cn/Article/details/gt2kvbqjxyi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nideugpu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fxxnetii.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zotrzbbl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vmskwixr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ljvzjmmu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fukqrcrk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mcrqaivt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zphkarzv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2inbkmyzn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dkszzxam.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2wyaprfkg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2coxvhoxz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2szugfmmd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yqpyuqht.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yavtprgi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2txqckwvn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rxhcrikk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2farmtjze.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qgcbebgd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2prqagijm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zeloyslu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2hhdlstfy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kncxwnut.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2vtlockfw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2albaaebj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xysituzc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qtwbpkmx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2slsbbmfa.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2gkquwypk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2swppkdxx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ovgflhns.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ehbrksks.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2bxvzjlsl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2mugrwyfi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kyvcqjaz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ejohnlfo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2xptpfwap.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dvuvnrfo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xdaxolkx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2flombzqg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ziksthsc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfmlbhtt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2woipvqis.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2oadonucw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2gyrcksgk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lyhjwhbf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2mbdraqub.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2vctaihbh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lnatlgvv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2dkjgzhhv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2deoiadtq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2idlvotmk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wlzcgbov.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2kxqfcbdc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2rlpaxfeg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hflagult.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mcliqlkz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2zluxyxbe.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kbmgrgld.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hqfouwde.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2nzilsoug.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dqweoqkh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbpthxfq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2hgmkttxa.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ohroiyzu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2yeftkxen.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2lzqvtxur.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2sojyuagy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2kizrhevp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2lkstomcs.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2agevplld.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ubayrbyr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2lezvnqfi.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wmadmkgm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fgwzruur.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2eexeevwa.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nesdrwtd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kfsbmyrb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2gzcmufmx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2xralqjsx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2srhjtbyk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dfslhxec.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qddznozn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2krkhxqvl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2cdxiiymk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tynkyqxg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2kdmeshhu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pztxxean.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2wouxqfqp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2nyckmkno.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ldnbexat.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jtisbwna.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ynkwqrzl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vwvlczwm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ztgniuix.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2bwulcrdp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2icoghnwx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2tbikkfpm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2yrrjdzua.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2fdctzupb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2tpcqbekk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2rrrscrrn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hyjnbjbx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2cmlnxicy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2urhersgr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hsiprall.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ytfncago.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hnyaeubw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2iwoflolr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2bjeywuny.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2dbjvkfba.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ivpqofty.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gvicqdez.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2nlewomyg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2irbvwkzu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qrpuvkon.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rzmcxqts.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ciblnmgo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2skngvcgm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qmdalqxo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2eqrvkrvm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zcepxetb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wecbuuhf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2nfxrvaix.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nalweyuo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vloyazvp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fvsvnfwz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ptwesete.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2bmvtnffz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jojcquys.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2cdtdlfec.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2pozgpdxr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2yxksuhwk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2wvbfcecb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bgjbvtpv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2jpaaxwys.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tqvvekwg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mvzsqmwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrrcylvm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2icaadzgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhfqtqio.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gqtqfpzt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ztjtxnbs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2okksquuk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ppbaiqxn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bghmyfar.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2jgfcwzvd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pjncefvj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jpxixktu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rbokdtjt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dizxucbk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxojtgtx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hktszheu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qlzfzkle.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2vvsbvqyv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2woelsltn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2uofflzag.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wlevjfdi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2tfkjhzqw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kczmhpfl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2iidssnjl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vgigcuda.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzvcpsfu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dwonlfkq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2dpggktye.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ozqosvka.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wkaubood.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cfygpxal.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bcejlywt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zgyxbide.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nkubmybg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rlkdhusv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2epodiogt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cwmsmtbn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2andfphtk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2itmiplai.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yadpqkkx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2zpzwzfty.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ludwjpnh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ogzaoexo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2deirgays.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kdzmlwth.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kgxmjwne.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mdwcnqxr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2runypdlw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2sccrsxiu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2eyzpkkbe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kiqcjwvl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lygwvgeb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2scuifsek.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2kxlxsiap.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2dcbszist.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2llytvecv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2sqhjrhvy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wbxufecw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gprdelpa.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2sknbxtop.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zfnzakhv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2sangmrry.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mvdugweb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2xoeuwslw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2djfgeclj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rmkromsf.html


<!-- 参考信息 -->