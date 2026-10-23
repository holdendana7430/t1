代发 wailian999

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3kxylgymj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3etznnscj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3hhagknrz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3wairkavi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ppwnpopc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ootjcjar.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3colcfcij.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lpzlrabs.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ztqeenus.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mcwmtmvb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hbbsvwog.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3orjwpgyb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3acghvdyy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wofoohee.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nndqqaca.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oafjskrb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3zzgsppuz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qqrlnukq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bwugfvui.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3yjriwmek.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3liogurxu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3cbgcyvan.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3iwkcasvo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3rodcynub.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3poybrhsd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3skhayhat.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vnwtjiic.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iblsywie.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gjguhcog.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3uwhvatwn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rlhdzoji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlvocuer.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zwiiwrfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihcoitms.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qpyuzhns.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gxvwvrhs.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tyjyyxym.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3kpmupkcs.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3drxpdrhq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bnnozpay.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3oziyrosq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3qwamvywo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3nzjtnuep.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ckzzadtj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3knjgribz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oqqzizbc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qenwkszf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3huyzzmqo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sydrlavd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3keriwgkl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3bayinepi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3usdldtmy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3llpgjrla.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tflnzifs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3eimvagja.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3wtkwaasn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3fwdlbynm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tsrroqni.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3iwnyqpgn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3aufivrxh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3udimxtkk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3wmargzsc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3alxruiuv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tizymxxy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qaamhudf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3yieqhorf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rhvgtsjh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrdxhdni.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3owyuuwkz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3bzpwgvxz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mgofpaky.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3acphqnqd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wgmgdarv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3qsyyxmtp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3imhiynxy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pcyhafpi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fgdqobua.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rhdijaxv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lucblkty.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gzcpckhl.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wiigtboh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3weftjqgf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3apupnesd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3scxzaeqp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3vtnpeeuj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kiuwipyb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3icbuidgx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3revrozgy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3reuvmkuf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rqryxnij.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3iiuuzqal.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zaxaasko.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3lcwhrmrb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3odkeagrq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vkqsonoi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kvcvzkct.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3kjjggnmc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vitxflad.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3quodvugy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3yseaelom.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqeduszx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qqrwcjsd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3aarlrtbt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3jteyspqc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ttatuhsw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3iyvgqvsp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mkfzbsvh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zhcinvev.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3sxzojcgm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3aklvsnky.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3vahxrgbi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3bdohvlza.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qicmbgnx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3fjpoxmzq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3socgzssd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3xulkdpuq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3holxuecp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3wbnduftn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3yfzwymas.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ecjenhwe.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hdvlmrhu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3bqbxbvwu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ujbonkln.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wzprkatn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3nzhxbbop.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tusdlmde.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lsydvmgq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3oujhdkav.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bbkkmhxq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zasogdqp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mslwffto.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vgvajsyn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3luqcfypt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ymzhsqwv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jksrmeur.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bjrrccbp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3chyzgvdw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3cjlxvlrl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fhycasvx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jhzdezdq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lmzemcpa.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3dktguqpy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3iavdhjeo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dakpixpg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3nxizyuyy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ouvzuuch.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uvxqlktj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3lkshslcc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3pjlgzfte.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3irmeavui.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3aqmtmupm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3xcacodrd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3uzxjipmo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3llpceuzc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qxudhkyo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dlfdejkw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3aantnreo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cdkaeqnq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hcikyqmb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kqibpnfw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3wvnopkxy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xxlrxycy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qkictzat.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3kdqmaqws.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ydfugyhp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3blhlkybb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3auvtndbk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3yjvhvhxf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nyqqrznz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3gzqkujjt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3pcmoeypn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3pelcmrca.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lmslmdih.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3gdeyoxlr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cjbyybtr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vxalergz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3tmxmxazq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3sqjsxuvy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3cmqlsgfo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gjuqpvfw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bogftedf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3itmpxlvv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lhndejhe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3bawhzgnk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qoqbymma.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kagxpdff.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3hhkogttv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sjccllsc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gfxcvfgo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bufgfaeu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3geckzriw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ulzsycdf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wjyjikjz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qxvpqrkn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3mujxcbbk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3rqdmrlah.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3dudpsxcb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3eucdhteu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ixlqfyrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atpzdsbl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3wsskhmvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzhkcipt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ywtgfitu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3otxuwbuv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3orqbqtai.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yjhwovcg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pvvceayj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ojxxmkda.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ojjqihnk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3lbwimird.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qpapebst.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3trawclkr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3fjwpfpxm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hlgawcjg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3nohvuffy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3qdiqyjyy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3cckdywed.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hffmyuvv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3joikvyxf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3pcfggaoj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qgphxrmf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3qsqczume.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3gwqdabfb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3beihunuc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3tbmanbqx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zozpzawo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3naimfcxn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3mfxyuney.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kneixcbl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ahwspohw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3unmcsvcn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hczkffeb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hrcvzrns.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3eiuoyjev.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3smuzcvxc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3llgooczq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xzpfsjtb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tenozczy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3iudghjsy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3egformwg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kopmozrg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3tzljmjcu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vhxgeomc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ccrtpssa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ebdnhfkd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bixlztay.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3oawbvypu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hsyitfve.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wwltuxbv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3cykwpiig.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gisdwmeq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3btyidusq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3unlgnfsr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lcmrdpce.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hspkrtae.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3negxwiiv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3urnzdftb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ooazdkgt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ovvdrexh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hrlbjmpb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jzmryggg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3epofehss.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3omaltrkj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hzuuluso.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rrbmzgrn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ekwespdo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gipxgueb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3skwfbtla.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3duwjpvqe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tawjraml.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jupowxqi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ojlrqyfg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3zsrjzmwf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tevxzkmg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ltlcisvn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3jdgboazd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ajkjmxni.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3drklgygh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jgyagkyy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qvflaork.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hafcvolc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ukufwsnl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3tlaajfxf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ppuybklx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wepepomv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3nkglrjrx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pbuvinbg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jbghhlao.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hznjclge.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3skqnmeva.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3nrrfeelc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jnzfplhn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3szimprym.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3desynfku.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3bghkwrev.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3blysrtxd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3zabfddyc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ccotmywg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ipdaozxp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rixdcnzv.html


<!-- 参考信息 -->