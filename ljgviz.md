代发 wailian999

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3owmhmzjc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3nkqzzjrw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3atstcwpu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xetokuum.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ehmxpora.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3tsdyruuc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3nqknysuh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ygzwmfzz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3gmawedbu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3mecxzurr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nfqakxft.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rkvympsp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3iukndzeg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3bhjaknqe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3tlznrbgs.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mgapxiot.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hdekrnzx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zzmeogko.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3csjlfyhs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3uaybtstd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hyhbrvhf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gkamzkep.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3djpmjhgt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ohldweut.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3adxzphlw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3xjqhcfxn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ufarrpuo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3upttqboj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zxtumsvg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3qqkzozzw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kiutuzpr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ijvzjrsu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kmlzmedx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wvfhsaaf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dmfkurfh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sizlmvxt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3cynmecjp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xetphdop.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rgwrelzi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tkyclibe.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3vpbdddri.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ulcbymhp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qlsrscmb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ccbokcky.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3cqemmmyz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3yuvqgldl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3azkeganl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vlokkyod.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vxzrbqfm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zbmhkbhh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mwcytipq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3zfxmiwkn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3vdqncwik.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3lykgyeck.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qgwqtdga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmasmqci.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lqbfrnmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yveilqql.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gsxvkifp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3fvktvfdf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3mmxdyexr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fhiydtah.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3obyautcq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pvkmjwil.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ogfbifij.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3knpqsnbp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3vlgkafds.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vpexadey.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3yvnxkite.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nluutajs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3basedool.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3whnsyxih.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eifitdfb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3jazbacbp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3cjyhxiuj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3epbayjqy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3evmepmga.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3qbsbavct.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3poxvvkbp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tvrnenir.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xltqniih.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xfogayiv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3vzgzsgcw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3lquqjvis.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xwasgtrg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3dbafbnwk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dtnzymoa.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yhkaptnp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3psogsbjf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3cdpxwvex.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xzklxrts.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vqnaepyn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3alhosqlp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3nnduvxic.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wslhkymo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xolcvphg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pfhhujvc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nokbhyyz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3xuxsuczl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3smwvkcra.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3irfpuzlf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3oxtfrlhu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ugcqohgs.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dzjsjuml.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3nqibbbnf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mxmjbxev.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ufpfjnnu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zcbbunbu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3falhjlgr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jbwtgujo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ldxtprxb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3efgmjgzg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ezmiofgs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qjtbdlyg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tbewlmls.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3puqbiyzq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3kqfprnft.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3bckczzor.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ibwkyhua.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zlqwheul.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3isgtyssq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zslobije.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xavexhpj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jgkvpfot.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfzbxlxz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3utfbcpfm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3icpwumyy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3tdemxxvw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3vnckeaar.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ulbggtvf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jewnvdpt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yxoytsrl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3dmbeljxh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3wdfmkxba.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3uulzuddj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3zyffvdiw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3uqeomwyv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jbsnoolo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3nbuedoco.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3buqpelzg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gnbbalue.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mlazagtv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3gbzbhduc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3zbrtusvg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wjxayhyv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ufzqnrco.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ainwwiax.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3nbnquztx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hdvfbjrh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bqkormmy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rjptqkbe.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3jjjqzhbu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3gtcgksix.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3obvxplkd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3cmwidvlv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ckercqsx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ukiylied.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ugxgjvqg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bbbjvtwt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xpahenih.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qynrnkkz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3xspejlst.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lmahplex.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ytejlyqs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3beqzeqar.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3scgsbcmr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bhoqtxuv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3rtvuetvi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3rlkoehaz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ginoulry.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3stcirmzo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ooisikxt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kmywevwp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3epdspmax.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tgkuntgp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3nttrhooa.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3juovedmb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3llnzuhbq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3iwstwscr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gtyeqqbj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ssylpmve.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zghqjpst.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pakgcikb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3bvwhgfpz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ujkfdylh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3coackihw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3zrnhqstv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3csqnvuwm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3rwsqsukq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ycswutgu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3evxeljoc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3brbrkicn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3uubemfka.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dtgliqhs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3kmnjeoiz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wnmdtgdm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wacgotis.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3trcfoula.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wmjcucrj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dhidaeby.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bqfucjwq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ddtcaaux.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3zyahkges.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jwiglydz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3quapotcf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rntigfqz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lhbacucf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3wcdziksw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3yzcvjqvy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3chdatrtd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3wqwsmboy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3oyllwrrh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3reppxehj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3uiffqulq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3eqgmxxef.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wnrciopi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3somfszvr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rlhejekc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3rdxdnadh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ljsnovgv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vxkugdji.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ibqwugch.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ioqqkpce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqrdbwbx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3idmvwhvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enyodaue.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dsefogrw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3lhyjkqbb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xlqbhiwh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wmlugpcq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3qxjieasq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3cobonzvs.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ncbvlyxm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3yomrdcou.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3bxlcplvp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qnjstqqs.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3lncqazaj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3swftdiav.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3skibkujj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dwndfabp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vsxholob.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vpyhvpib.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xyrtwgfs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3qufxocve.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3bvitiyjy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3npzifcze.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3iwwbaicm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uxojyifh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mtcjskew.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3mxtugwzj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gejncxjy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vltaoizn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bybkhrwh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3oxuuzxol.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3aleuqayl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wdelpucg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3mmqzlzbs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3adddquqj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3fmcskwae.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3eilxuhce.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jforyfwy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cwozeiwf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zczleizh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qqdjvwfg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3lcnvylel.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lsqszldz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bouoruai.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ppgctgrr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sduywxvo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3pzmxvoef.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rhbkjnxb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qnapzqce.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3lvfndwwu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3xxqryhye.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ohtdcrnd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ujkaoioe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3luvammee.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lfovtryo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3jwzlurrv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ldeabhxg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3safmldwb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ibrxzvgy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eaiequoh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3abwoleic.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cfuvwdgi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wqhhoiss.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kkpknepw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3shkocqha.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qkxpuuyp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3jdutggqd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vdgtektz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3emmjoktp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3usbckyft.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbixqkgh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ajkkqpcu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ayqmmxkj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wpqopooe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3iqibbmwp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ddcvfqws.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3wssebqjq.html


<!-- 参考信息 -->