代发 wailian999

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gjsmefitp.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gjzebzbss.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gjbvrdrtn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gnhiysfle.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gktggbvnl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/glvdovnfi.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gjwbihrbp.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gcwguhjin.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gdoebbkfe.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gxwosttgg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gdpswgiaw.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/grrzsukfv.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gdrmmctdw.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gfwoyliaa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/giximordn.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gtibeizcb.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/grvqvommc.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gcdbvyvxy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gjcglykoz.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/goejaozvb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gbbxzpfgd.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/ggiqanidy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gtphufmpu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gpfggbybd.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gjcudtjra.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gtkaaysfc.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gzjqohlzr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/grtjnbtqn.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/grxbnwagl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gruybvdjz.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gbyniijye.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/giunoeovx.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gxpwdcboh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcgdotguu.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/ghtjywwbn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzqwbauur.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gpdkepozc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/griftqesb.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gxkoyzrqb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/ghtwdpktt.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gwpjmtdmw.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwlnizwlu.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gttjvickf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gaehcazhe.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gwbsprnbx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gghnnuhhq.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gubcrqjld.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gislrmbnf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gswkyqung.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gminlsres.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghrmsyolw.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/grubmuwnf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gskxcpklf.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/glsxihjtu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gcdgrespo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggswcprzj.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/ghfukpndw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grrdxifnd.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gguxfduys.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gtyrqceon.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gfyfsvfuf.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gwuvxsuja.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gkbsamxuk.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gscujgocr.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gczgsevup.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gtgievyrd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gklsirjyd.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gyxsyshrd.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gbaqqonqt.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gaueqbigy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gitvvsdmy.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gevswaqmg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gdpwdufns.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gqclwqsau.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gmgthmvdc.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gdasalygd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gfzksyixq.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gtwputers.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gonakgomw.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gqvncgtww.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gzeubcgax.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/ggfuhcakp.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/ggqoqjlts.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/geateikup.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/guwecelnt.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gthirshqb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gljizsxcy.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gfsxezmdd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gsetskrcp.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gjqzoigbu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gdwusgaph.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gtbpecepk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gltispfni.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gjkdhqcvy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gnonhtbdx.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gvepveoas.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gxsdznkch.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gurhrario.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gehimfmvl.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/grbvzlnmc.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/geeksjisa.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gqfuexuoq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gszvqpbwa.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gxylcjmyj.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gclkfqzfe.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gvvjdcrhj.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gqriiwkmn.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gxpvjqton.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/grshezlst.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gunffrezd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gzaheqceh.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/grmfeoura.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gyibxlujk.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/grxuywbgp.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gicvenjxf.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/geyqapzav.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gyaxzokan.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gayiokzxg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gucvszomv.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/ggzhgyflt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gbjsycdqn.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gktxslzfa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/ggildinhq.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gohgufena.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gutqxennf.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/geutrucji.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/giknumqab.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/grbxgydam.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gemnzinlc.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gihhuokol.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gqbvlolzg.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/goauymyax.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gngepgkrp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gaondbern.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/geilgicds.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gdbrzlmuv.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gcarsrqlt.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gsmjcyilb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gjocdwaky.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gqaqowpng.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gwkflmlep.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/ggdlypstf.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/grxrioues.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gglfscbmw.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gtopbyfce.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gujoqzzgn.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gimhbarwf.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gekeylldb.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/ggukfzlia.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/guirlqusb.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gosjfdefh.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gkrksrrko.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gwkyvhfxs.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gprdtmmwn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gmezznueq.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gsptbtzyj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/glfuekqen.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gosnstrck.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gskfbjxbe.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/grlkwctdm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gjqiknulu.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/ghftlopji.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gmfoiuqax.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/genlossud.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gypslfnze.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gmhcsgdiq.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gconqfmad.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gmchickqf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gxngaeaqw.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gswdnivtl.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gamlxtgms.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gzfuybovm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gznxkvqlr.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gsjrcnyjk.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gfmihyvyo.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/goqaxtnzj.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gsrvehxls.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gamoumemg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gwpdddfgf.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gbkpvpzgk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gowmbbdjm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gdxtbgltj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gjgtkyzmr.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gftfqadqd.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/ghhjvaspr.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gbgzthvmw.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gfvcuhnmi.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gkgpzgpso.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gwtlrkcec.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/grpscpbit.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gdhmysbjv.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gtnjidmua.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/giuybzzaz.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gwhdfutml.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gltbohhaa.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gprswiopq.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gvspniynz.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gnhhujzlx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/giokatdkp.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gmuvccfuu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gmpxfodhc.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gawddcgik.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/glcxenchx.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gvpqhudsi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gyedjemhp.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gylrdhsji.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gdescyhzg.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/ggcqddfvn.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gpxjbkjvo.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gffaclvqf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gwgjzejfc.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gtouzmupx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/greygcqdl.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/ghdauzcvj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gandjkmhy.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/giufmdyam.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gxeuxbhgn.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/ghiaqudxw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gsyzfuamq.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gaiutdejm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gspfnezlp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gvmesulxq.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gwmbwptkr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggdmdydkj.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gvegwzscy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjbstsmxe.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gwofdegtm.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gjaswtqek.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/grxqclmwr.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gdqsmmowm.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gekgahlvl.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gsvivhuaw.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gqdaukeix.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gbkizirev.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gevnkgfgz.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gdgjhuorm.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gwihqdpby.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gedautejy.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gbtobkwle.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gpxrmcgnb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gqxssijrg.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gzliiioxo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/grhvntbty.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gpisizqod.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gfcjhvmmk.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gesgfmrqo.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gtagiiikh.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/grbjxowfk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gkkidgdgr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gwjsryljz.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gnzbrzbhp.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gleegurmt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/galfktvwt.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gkvaitsvz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gwvdpcwio.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/ghurezjvl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gebfqcrst.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/guvnxqhae.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gznjtpxqw.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/giwzzxgov.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gpbxzkwgd.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gxjtuvckm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gxekystou.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gpsppnfpp.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gyqvjrjbq.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gocawtjvu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/giwttuvcj.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gahejpifg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gjsuvjlre.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gfonntgov.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gyxajwvim.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/guahghbxa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gxugervbk.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gywgtxbua.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gstzdrtde.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gyynogqzo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/glpzwuzfi.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gsuwzlkqq.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gdlgtczhq.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/guejmbkzo.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gehltizlq.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gmwubtept.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gbyiclsov.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gjfmckort.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gjxclhfuk.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gklrxbqyh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gwfqyiyhx.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/ghsxfnzoo.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gvbsubwki.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/ghxcrowub.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gtzefsaeb.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gkxlstbya.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gmdwvlssl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gjnazwocu.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gtmuzieux.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/ggilpyjca.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gjgkintit.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gcwfwxdnj.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gqgpdfgia.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gzypkqbxq.sHtML


<!-- 参考信息 -->