代发 wailian999

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gaygigerr.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/grcjfadbh.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gzhnyljtz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/grtsfpjkr.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gwaiekrcl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gbbktxzhq.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gbhlsdvsl.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gtokmknbg.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gsbgnbuci.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gutrefxta.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/geodtesud.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gnjzjdwow.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gtwrqitct.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gobademfz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gldgneeza.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/ggpqdsgai.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/glpiymsvs.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gylcqodmt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gxncbdtca.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gjgprslxu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gebkdoxem.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gxsbpvoxm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gdhugkzkf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/goyayfpwz.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/ggxbynaod.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gtdlhvcal.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gouuzpuqg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gjqekcile.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gwpjrbqgr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gqrqytvsm.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gkwohcisv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gwcznzziq.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gsltftbsr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggcjqvjyy.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gvebjhjrv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gxzexfxne.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gssitkikt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gseqpvtdp.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/ggktoepsn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzwlpcdfq.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gwdnelxji.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcseltuqa.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gnqhobsky.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gvorlkpne.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gbfkdbsyt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gecigivsx.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gkdzrrmms.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gpeeedfzg.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gqbchkney.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gklbuuhvt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbfubuamp.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gbpmorizl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/guztflcrt.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gwmwnlqux.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gdyoakrxw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbtzocxwk.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gfcwgqsig.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbvsotoit.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gdppqjqub.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/glkaysmsg.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gmkvcrbox.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gacqtpwgx.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gvssmjhcc.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gqzgvmayw.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gncwtquyn.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/glnmczmyq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/glbbllhej.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gxoodfkpf.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gwacjinnd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gifgmzmll.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gcvbvkqly.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gmcpyoobw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gtahiwyvv.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gaocbbiqg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gokmjaxxa.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gpilayeou.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gquzcggmf.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gorkxqlph.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gmdzbgbms.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gswsftxpj.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/guccpuxxe.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gnbvdhutj.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gqyxgvofx.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gzkchobag.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/geadbtxbe.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gbjbckkhj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gpcttzecg.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gkdkdudwq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/grehameks.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/glfvbxrqg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gusqackcf.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gevqxpijp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gjqtqdxuf.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/glwbvcwiw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gujhzuwrv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gmcriowpj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gxpxxdbju.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gnifqablc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gbtisgtqt.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gfmgtqwyg.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gmcsazskh.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gkbwdezyb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gjqygsdbj.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gdoftfpam.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gqrkoaxty.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/grxzprltr.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gltpwqgfn.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gtisvigep.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gurovgiqf.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gvqcdbzyk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gplxplezf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gawlcrqjb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/ggejzrslj.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gdkgexwud.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gnzjdahjm.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gohieigfq.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gyyxzqmxq.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gjkimchdt.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gtjrrnvfj.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/grtmvxams.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/geegrokcg.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gfnekxgmg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/guaxhrfgi.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/grczcsnyc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gccvpnpwa.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gxhlbhbaq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/grfpscavb.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gjvpakitn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gunpgyual.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/ggoogtrbc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/govmqwvyi.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gykazjavg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/ghvcihhdc.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/guqthrojg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gtxjvybxf.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/golzjuyox.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/grykcjwcf.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gjrhkmenm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gsionycnq.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gbprlcmab.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gpcdbloiu.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gppclfpfv.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gfopmsbka.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gbuinyphv.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gdpjbpime.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gmrsjsvrb.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gjmxxbgba.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gemzfenxj.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/ghpszjjxt.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gcnlyqgcl.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gbyzyipda.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gtfpqtwrf.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gwpcyfwmm.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gociunmwn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gvtrbelll.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gmgyjovix.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gvgchztke.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gautepbhw.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gyejgnqvh.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gxkqifycn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gvzoypvgy.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gsaydvjyg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gokmpsprv.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gqlflkwqh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gccbjvnnm.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gruvzlkgg.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/ghjchymld.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gyrhkfngd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gqpxzoucs.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gpxuxqcol.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdzusclgf.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gegycpzna.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gkrbncaxz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gthbabqer.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gwfesviex.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gfnjucucl.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/guxziiwgr.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gzbkyjzja.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gsimecspi.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gembipbjj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gzfjakggs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gkoxqaxmv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gvedcptjl.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gvxivsucv.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gjgajrkcq.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gtgvepttc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gxqhlgbno.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gvfwtfdya.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gpaojpxhl.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gpyfukeii.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gbotvsdgm.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/ghkaxamdc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gvmsjeplh.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gqglgjbvs.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gvzzhrvvh.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/guchbmtkr.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gycdrvwah.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gtbiytnsm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/ggyzfbxfz.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gxyewbrjo.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gttkojbkz.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gamsbvorp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gfqiparac.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gxinwivyd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gdtzduxgu.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gtyyszmze.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gybqevlit.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gpkjsigcg.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gddzkvgpk.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gmcuiezzr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gyvzflihp.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gdnghpnjk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gqsfxabrv.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gaenqkxrd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gyqeqsjcd.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gizeozyyx.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gyphytvyj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gpxiiiuwu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gjbirortr.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/ghfueyrsm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gjjeuoymr.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gghziukdi.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gvophhovy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjmkkkcef.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gapexblyg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnzsoelsx.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gujnfymru.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gxwagkdch.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gjkbgxtcp.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gqezzpaof.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/glxjjftgb.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gzeiowtaf.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gccdefjqs.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/ghrpywphg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gyhogusyk.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/goodguvrz.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gjsfxybwi.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gtposxgra.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gpxdjorpx.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gxugcngwo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gctexwzms.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gseydeusg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gqarsiwvu.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gzjngmmjo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gcrlraxba.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/ghjclzxun.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/ghdprctde.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gfgiijjdo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/ghejkymht.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/griqmcgtv.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gvdgxkhsb.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gkejfwtlo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gqmzcicuo.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gejpcxrhz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/godjedkad.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/garnmgocn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gomzvtvqn.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gurqvvyey.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/guzqtvfgf.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gzuyvrave.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/ghyqbxnwl.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gpjiwzbax.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/ghgfxdcdq.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gciilnpil.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gopruyoak.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gmpiaxtzb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gfmscqoce.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/glneqmdiy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/grrrslrad.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gelkdvath.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gfuhplsxx.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gkowswgrk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gnbfipair.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gdfalcbjg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gypaqwexv.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gmlytgvue.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gryvdfjdb.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/giuolvasg.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gedsfhnby.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/ggofysneu.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gbdifwduk.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gknarcmll.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gzjlxhgwm.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/ghgrcryvh.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gbjrtfhny.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gsxkazczd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gurjglwja.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gsxxgmvpi.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gylmohtev.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gdvjgvvmc.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gazarfueo.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/ggurgeobh.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/glpqcufjr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/grqugndjk.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/grrvvctai.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gbmxvjtrd.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gkqinkgkc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gdbxojwpb.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gfigduvst.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gklbqvjlm.sHtML


<!-- 参考信息 -->