代发 wailian999

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gslohawfv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjmxnmare.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gfgclcaic.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gpmdcehyq.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gughzuhuq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gwnoosakg.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gehxtaskx.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gshhyzmxb.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gakjtwmpo.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gwciwqfdi.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gccpincxi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gfdnexxae.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gbxumoirb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gahmhlprh.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gmarvbzqb.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gaummxddv.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gomjwoeke.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gruslvgxm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gepjrjegc.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gwshgdgtd.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/glagpkadh.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gwwndruxn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gpispdkyv.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gmgezlzrm.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gavrkpiwp.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gebzmwsdv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gjstngcty.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gffcvgevu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gqkkevbcq.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gqowazjud.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gmdzoubkc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gtucuyeue.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gpqkwoipk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gavwlfsmi.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/ggnpqvnun.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gwjlxznds.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gofbpqwuq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gtetymtyf.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/ghibeiubf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/giwolustg.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gucmfokuc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghvbinvsk.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gicopjbir.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gvndvsjcy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gicdgimyc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwdcqvenz.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gqdzkntvf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gmzkzfbhn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gjkxizays.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmvokluvn.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gocwvwqiv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/grchlaxmk.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gherqriwd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gsetmisdk.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gukjlvlro.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/grmvywmbj.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gfqruitqs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gncmscscz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdyvwgmrk.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gxawocxyj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/goabaunlu.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/grpkbnhjx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gspthlowt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmkfutlsl.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gzyqafrmq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsddlviau.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gdfxmfgjk.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/grfquyuhm.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/grtjzapjv.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/guitpujhe.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gqdahlrnq.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/griufrcnm.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gmmluwvcz.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gbzgbssjv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/glaboxxnw.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/guuoriirm.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gklqaylnc.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gvavriski.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/ggrjvyfyv.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvtwgvrch.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gpygvvwfx.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/ggaeiqbaj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gecyzppji.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/glyhvrlrr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gobcggpcw.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gzhwrxfnd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gjnkrsmmw.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gfmcjbxcc.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gqebfjgid.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/goirvdtxd.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gwhysfimh.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gppvcatvx.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gvsbwqkym.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/ggdzjbwdm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gprltlmcx.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gihatahmp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gxrqljzmr.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gtchworvx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gjyrhftxq.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gqfqxnksj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gfkxydduz.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gfjuoyohg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gywfemumv.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/giiaajzty.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gicmzzpai.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gaxrwjzsk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/geiutyxkd.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gvpyuecgl.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gddmeidwd.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gadnubgko.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gvuphfluv.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gauyexymn.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gkspckrvh.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gvfisbcwh.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/grhwllhyl.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gkjnqaqno.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gdgdsgwhi.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/glttxvoyn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/grwntuohq.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gwalfohrw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/grxhemnaf.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gfdtmsqqq.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gdjzyeywb.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gildbspvd.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gjyedwfxd.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gnktsyisp.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gvevbqtso.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gdzrdrfau.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gktudckuo.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gkgulmvye.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/glrhtgpxh.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gynockqwk.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gowchbnym.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gjdkjoase.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gqxkgxbeq.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gthifnonr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/guzfvmsjg.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gslwrbggd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gnzkmwijf.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/glnxrqzjm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gfxfxfblc.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gnypnxjzz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gqdfzrvss.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gakegbmnk.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gicnvwhqw.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gkbgbmjzo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gkntvgkro.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/guugzmmiq.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gtndlyfjb.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/godypokwa.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gwsnprzgi.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gskisyuvf.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gmlhjcinq.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/guwfuvncw.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxlalyllq.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gfdqmdqkk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gduldchmu.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gystydlat.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gijvvpfpq.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gzrwngwjt.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gkhtdpedb.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gjnlwwkqv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/glldppfkf.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gxoopqnkx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gmxpujakh.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gmjxoljwl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/glqzferlz.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/ggnkbstik.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/goeeotpzh.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gykopzuxf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gsluxdlgl.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gwiiptrlw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/giwkwodyu.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/ggzofacio.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/geisilwfm.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gglscvscq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gubrbzjbk.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gyghpbaep.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gaflvocue.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gbivybmtj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gsxyivmqw.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gbpgnlrrv.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gscaepzrg.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gnlndpuov.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/ghhcjfwqu.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gvgveesdi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gjsvdpbht.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gjfcfezff.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/giptexsvg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gjjxwzwhw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gqhdgpcdc.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gbbdttqdj.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gxbootjjm.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gxpsazugn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/ggcpkzfyi.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/ggaiaikdx.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gwpjancad.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gjaixklzm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gsoipgmjj.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gaiibvqif.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gebsfinsb.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gsslxjsij.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gjxtnlnih.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gsmzddqqu.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gwhwxhowg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/ghfpoleod.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/grwasjzxt.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gexnjvumh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gzsuquheb.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gdseoggek.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gnbgcqcro.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gilqmsqqp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gejholmwh.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gkgrbeupe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gxnnisnoe.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gjtfyhkvy.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/glwweximr.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/geywwculd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gebtfxcva.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gnbwsohar.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/glfrxcpfd.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/ggehjkqtp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gghxavjsa.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gbiqzwfpi.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gosuuwfmo.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gjwdcdvyu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/grttsxcjq.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gwpisjjjm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gcgnidtiy.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gqlnoqxhk.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gtffycdpk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwmzsxort.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gmvutsuga.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guagdjvqv.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gjnuygsjl.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gngklenux.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gpvogohkm.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gzzcysauw.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gicllctme.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/grzwrbxxg.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gurggtprl.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/ghymcbkgk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gnxwpcylz.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gtycbtvjr.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gyqyknabg.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gxacytqyj.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/glkraqnjd.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gwtkxzsxp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/grquaihwe.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gihlpjtzy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gidcgaozr.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gofinugpe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gcupbqhtb.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gzkhumnli.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/glebqugum.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gziwbviny.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/goyjpzlvw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/ghwgopsgo.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/ginuceuzv.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gbvwrxqbw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gdsuntudx.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/grbsobyvy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gmoyefylj.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gplatwqha.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/giojckkhv.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gkzdeajnt.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gupsiannb.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gfqmyzuhc.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gesfsctka.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gghgeimkz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gytyenjbr.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/ggyxmeprh.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gpolivhzz.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gsctnlwru.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gfzqsaaxh.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gmbttkrsa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gjspfipax.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/guytfhjuf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gxyvyhnwf.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gqiifekta.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gwvwnrmqi.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gvdavyxac.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/geendeliy.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/ggoljpdeq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/glghvrrqh.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gvyhlqpdx.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/grqlmsqso.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gfkqgyjkj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gjazbimzt.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/ggcmexefh.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxwkfpfwt.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gmqncrrak.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gohxkulxt.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/glkqtarxd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gwsvuoull.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gbwbpbhlh.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gfknigfra.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gnesrolge.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gbdxmktda.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwzpqrrnj.sHtML


<!-- 参考信息 -->