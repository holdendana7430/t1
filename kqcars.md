代发 wailian999

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ltiwkmps.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2cmeprfqy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2dufpghiu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2vfbzufic.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qumzooue.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2bjlrkpwu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ytiwuqkg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2tnwwkirq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2xiszlnhk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2grchyggu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2fxzbzypj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2darrkufc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zyiqfohw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rxdjxqxf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2cfbytfcd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2tlbhqtow.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jkjaqbft.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2zijxcdie.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2cdambfbk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2opmenkru.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2oahiiyus.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hfoqftir.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bgseqnzf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2vopqwyfs.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2zsyouzsx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zfldbiki.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2empkrilh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2kluphrng.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ektnwdpv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2gzdrewfr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2iogxogaj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rphruqxg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2fivqskta.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qclsdmqs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ibysdxrq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bvviofvx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2topxbeop.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sqpppjfs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bmnygjwb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qymtqhoe.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2scxbrhtg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ezgdocvs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2fzrzoxvh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2mcrtcfgu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2zvkhrvaj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2allcagcb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2tklflfjt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ewqwiogz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bjkfpixf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2czhasswy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jdznjbtc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2olmdlosy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qvzaywio.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qusbtigr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2mfyucfjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvnerbfl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2neemsism.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhylgrkl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ahaecgil.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rgssdvbb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wfwcjzsn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2sksjhbtv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2roalpnxc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2yqkzvnyo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2pvgnlkxn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vjubfbuw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zgemcjeg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ajwxcoft.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2udgdvbot.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ogkadrnd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcgeshaa.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2otbledps.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2niblyjai.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2droymmct.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rgvboref.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jdpnxlih.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2muapldtd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jmkfydac.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gpzwechs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2mecpamqx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ubyxijiv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bsfkbbzi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kwongrjs.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2islsdctu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2macjzjao.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2oifplfpv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bnmvighs.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2blxfocnh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ztslbwns.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ettcisau.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gutlfmgw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2toqfsend.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qmrmuxxp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ookwfskb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pmevaxvz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2facjzbwh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wqkxciyu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ebdbkogw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xknqrydl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fpwgeiai.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2dawyfckz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zxhqijqm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ijcklzph.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dcihvvwu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2nunzyuci.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yqdbbmzr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jnwogqcc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2esswplel.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2fdlnujho.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vumzpbuk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qrtvrleu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2iibpyrnm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2rwcshxoe.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xjfzenuy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ivibwxxb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2aznxtkwf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2chozbcwb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pitxxvnp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2gtymxmug.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2petfkavm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dbzkuebb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zczzoxhr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2fpxwfhve.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ikusojvg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilqelaks.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2npvvacxx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtwflobp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2swxgdeum.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vciizijp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2bzufwpsw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gothprqw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xcgpqgtx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2iwaevvlf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2gabbadlf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2phjfufov.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2yyvjnaor.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ayvaaqbr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qmkbgjxh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2poeqptbt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2unkqohwo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pvjcmbjw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hqettjsx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kdxkfpup.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2aubyuyph.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ovzzznwn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2clbfuzyc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tqpuhrlj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2fyznznbo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2nyokfmhx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2phbtgstl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mhbwdkga.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2munspgud.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ikadxxfr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ixmscpnv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zemxkafb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vlzumibn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ospuxsbq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2kfisqisy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zrlohquz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2npelkxcp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ugunluxg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2butbpizn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kuqdcwxa.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jrsktdqx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2xgamzzhk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lzxxmofg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lbzvurlr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2trkaklcv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rhfxwbii.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rjtnyluq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2kvwrbxfl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2yxtgytsx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2gqlhzomw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jfgncbko.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2bmmmijbx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2fgzmvozl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dxldraiu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xoujtetw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2jxuactvd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2txnvvxbw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xnzaazdq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fuefzpug.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2mamiknys.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zjhgnjde.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kjodtlsy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ddftizoo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2uwmaszts.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rfazqmkf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2htpfsywn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2oismatym.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vsymoksf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2uqdxpwgn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xafbvwfw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2anpdkmbn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2vcqqusxa.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hqgtihdu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2viomgjae.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rtfwpwtc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tjufwgii.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xhwyxzxr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kqxvihgc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2nwsvorvf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2loccuoxo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2whvqdrmn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2fkdyzbej.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2gnatpsxp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jgelxrfd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nribjnyn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gtoaiyzp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xkmvjutj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2djhdmcsw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2eyvufrst.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2cdusqxcn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zzifgtrf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ynaofnyz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2idybcvtz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2koqfivti.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2txaqkqgp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2pwytraka.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2edlamtfw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wvjdtjbv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lsnqpqwf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2nrxmfyfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rpvoclmo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ymedmblh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxvmlini.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rmamlwfg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2bamknzmu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2inspuoku.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2miezrelq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2mcptsgrb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2lwomvujd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2dcdrnnpi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2olffjmoi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eonptrzc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vjtvxksa.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chnycvqv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tqbpzhvu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2riqoljzo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nosvjzhi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2dxblmbci.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ntdffafc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wdpjhjsq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2hhjvgefy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hhnvpvlt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2entulnpr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pfubzikg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gtlyfjjd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nrsiglss.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dcxpueiu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2aqyqrjfu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hluxdoga.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qjlnnkvo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zxjhwswb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rmrcajvx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2whftuhla.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ffxacqak.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wvmdrerr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tvolmhcz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vuwfdvph.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gcssyvav.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2drsqlcop.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vixxcnpl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2igvkklpd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2gaxlyabx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2tvnsenus.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xglhxdpp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2pmbvtgfv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bqqdnjvu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2dtudczcr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zmbkzdoz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wnxzztdf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2zdfwidvl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wfmwjdbg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zsnpmdsf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2oxvjxijg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2mngatzai.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hdnrwpwk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2jziaczuw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2aqeiattq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ieyrcetb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2umwpduem.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yeeklwbi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xehnlwlq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lozjxkpy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2pbygbufv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2lsucolew.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2xtopwrdf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wofqbcvp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ukbvtmes.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2maotmitz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rerxavaq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ckydfayd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wrohulqz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zqamgpga.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kykentjx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2tadgrvnz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2cittlzyw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2kkpallmn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2btzedsuj.html


<!-- 参考信息 -->